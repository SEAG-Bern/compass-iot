# Compass to IoT Platform

## Quick Setup

1. **Create a device** in your ThingsBoard dashboard
2. **Copy the device token**
3. **Add to GitHub secrets**:
   - Go to repository Settings → Secrets and variables → Actions
   - Create `DEVICE_TOKEN` secret with your token value
4. **Access the app on your phone**: https://seag-bern.github.io/compass-iot/

## How It Works

- **⚠️ Must be accessed on a mobile device** (phone/tablet) to use the compass
- GitHub Actions automatically injects your device token during deployment
- Compass data is sent directly to your ThingsBoard device
- No server setup required - runs entirely in the browser

## Security

- Device token is stored securely in GitHub secrets
- Token is injected during build, never in source code
- Can be easily rotated by updating the secret
