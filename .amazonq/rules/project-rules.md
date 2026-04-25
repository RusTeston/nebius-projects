# Nebius Projects Rules

## Project Standards
- Always follow the Deployment Discipline Agreement - require explicit "APPROVED TO PROCEED" before each phase
- AWS region: us-east-1, Account ID: 901779867920
- All projects use static hosting (S3 + CloudFront)
- Design system: navy gradient background, Inter font, Nebius Canary (#E0FF4F) for branding, Nebius green (#00C853) for accents

## Deployment Patterns
- Splash gate page deploys as `index.html` to `s3://nebius-projects/`
- Projects landing page deploys as `projects.html` to `s3://nebius-projects/`
- CloudFront Distribution: E3K7BNEXGNYAIR (nebius.rus-teston.com)
- Token Factory Lambda: nebius-token-factory-proxy (Function URL)

## Code Practices
- Keep responses minimal - don't be verbose
- Read existing project code for patterns before making changes
- Match the established navy theme and design system across all project pages
- All project pages must have "← Back to Nebius Projects" link

## Deployment Discipline
- Minor changes (comments, text edits, doc updates, small fixes): proceed efficiently with approval
- Major changes (new pages, rewrites, new infrastructure, new projects): follow full Deployment Discipline Agreement
  - Propose → Review → Test Plan → Rollback Plan → "APPROVED TO PROCEED" → Execute → Validate → Document
  - Create mockup/preview before deploying to production
- After confirming changes are working, always commit and push to GitHub before moving to the next task

## Safety
- Preview HTML changes locally (open in browser) before deploying to S3
- Never deploy without explicit approval
- Always have a rollback plan
- Clean up temp files after use
- Back up current files before making UI changes
- Before any CI/CD workflow that syncs or deletes from S3, compare S3 contents against local files and download any S3-only files first
- Never use `--delete` flag on S3 sync without first verifying all S3 assets exist locally
- Never expose API keys in code, HTML, or GitHub - use Lambda environment variables
