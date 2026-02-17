# Deployment Notes

## Surge Deployment

The Virtual Office dashboard is ready for deployment to `henry-office.surge.sh` but requires authentication.

### Authentication Required

Surge needs either:

1. **Environment Variable**: Set `SURGE_TOKEN` with a valid Surge API token
2. **Interactive Login**: Run `surge login` with email/password credentials
3. **Manual Setup**: Create `~/.surge` config file with credentials

### Deploy Command

Once authenticated, deploy with:
```bash
cd /tmp/.openclaw/workspace/henry-office
npx surge . henry-office.surge.sh
```

### What's Been Done

✅ Dashboard improvements completed:
- Added Budget section showing token usage rules (70% crew / 30% Shawn buffer)
- Enhanced date/time display (local AEDT + UTC)
- Made activity log section scrollable
- Added nighttime/daytime usage strategy display

✅ Changes committed and pushed with author "Shawn D'Souza <shawndsouza@outlook.com>"

### Next Steps

1. Set up Surge authentication
2. Run deployment command
3. Verify deployment at henry-office.surge.sh