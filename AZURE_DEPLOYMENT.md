# Azure Static Web Apps Deployment

This site is configured for deployment to Azure Static Web Apps. 

## Deployment Steps

1. **Build the site:**
   ```bash
   mkdocs build
   ```

2. **Deploy to Azure Static Web Apps:**
   - The built site will be in the `site/` directory
   - Configure Azure Static Web Apps to deploy from the `site/` directory
   - The `staticwebapp.config.json` file contains the routing configuration

## Configuration

The site includes:
- `staticwebapp.config.json` - Azure Static Web Apps configuration
- Security headers for enhanced security
- Proper MIME types for all assets
- 404 fallback handling

## Environment Variables

No environment variables are required for this static site.

## More Information

- [Azure Static Web Apps Documentation](https://docs.microsoft.com/en-us/azure/static-web-apps/)
- [MkDocs Documentation](https://www.mkdocs.org/)
