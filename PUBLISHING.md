# Publishing Guide - Chapter One Theme

## Quick Reference for Publishing Updates

### URLs
- **Marketplace:** marketplace.visualstudio.com
- **Azure DevOps:** dev.azure.com

### Local Testing
```bash
vsce package
code --install-extension chapter-one-1.0.4.vsix //the same of the last version published
```
Then reload VS Code window to see changes.

### Publishing Process
1. **Update version numbers:**
   - `package.json` - increment version
   - `CHANGELOG.md` - add new version entry with changes

2. **Package and publish:**
   ```bash
   vsce package
   vsce publish
   ```

### Token Management
- **Owner:** nenets
- **If token expired:**
  1. Go to Azure DevOps
  2. Create new token
  3. Find marketplace section
  4. Grant "publish" and "manage" rights
  5. Name the token
  6. Run: `vsce login nenets`
  7. Paste new token

### Version History
- Current: 1.0.4 (July 18, 2025)
- Next: 1.0.5

---
*This file serves as a quick reference for publishing updates to the Chapter One theme.* 