# Misi Pulau SKUAD — Avatar Creator Upgrade

## New student features
- Avatar creator during student onboarding.
- Editable avatar at any time from the student island screen.
- Face/skin-tone emoji options, hairstyle/headwear options, hair colour, outfit colour and accessories.
- Live avatar preview before saving.
- Avatar changes are saved to the current student's Firestore pupil record through the authenticated `update-avatar` API operation.
- Demo mode changes remain local to the demo session.

## Backend
- Added authenticated `POST /api/skuad` operation `update-avatar`.
- The operation uses the existing authenticated pupil membership and updates only that pupil's avatar field.
- Existing session, response, teacher and activity workflows are unchanged.

## Deployment note
Deploy this ZIP as a new GitHub repository and connect that repository to a new Cloudflare Pages project if you want to preserve the existing assignment deployment. Configure the same required Cloudflare environment variables/secrets as the current deployment, using your own Firebase and Gemini credentials. Never commit `.env` or service-account secrets.
