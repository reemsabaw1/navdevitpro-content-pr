---
Module Name: Microsoft.Dynamics.Nav.Apps.Tools
Module Guid: 00000000-0000-0000-0000-000000000000
Download Help Link:
Help Version: 1.0.0.0
Locale: en-US
---

# Microsoft.Dynamics.Nav.Apps.Tools Module
## Description
The [!INCLUDE[nav_dev_shell_md](../includes/nav_dev_shell_md.md)] includes cmdlets for creating extension packages. These cmdlets are included in the Microsoft.Dynamics.Nav.App.Tools module that is installed as part of the [!INCLUDE[nav_dev_shell_md](../includes/nav_dev_shell_md.md)] when you install the [!INCLUDE[nav_dev_long_md](../includes/nav_dev_long_md.md)].

>[!NOTE]
>Also included in the [!INCLUDE[nav_dev_shell_md](../includes/nav_dev_shell_md.md)] are cmdlets for merging and modifying application object files. For more information about these cmdlets, see [Microsoft.Dynamics.Nav.Model.Tools](../Microsoft.Dynamics.Nav.Model.Tools/Microsoft.Dynamics.Nav.Model.Tools.md).

## Microsoft.Dynamics.Nav.Apps.Tools Cmdlets
### [Compare-NAVAppApplicationObjectLanguage](Compare-NAVAppApplicationObjectLanguage.md)
Compares the language text files in two folders (original and modified) and calculates the deltas.

### [Export-NAVAppPermissionSet](Export-NAVAppPermissionSet.md)
Exports the specified permission set(s) from a Dynamics NAV database to a file.

### [Export-NAVAppReportLayout](Export-NAVAppReportLayout.md)
Exports the specified custom report layout from a Dynamics NAV database to a file.

### [Export-NAVAppTableData](Export-NAVAppTableData.md)
Exports data from a Dynamics NAV database table to file.

### [Export-NAVAppTenantWebService](Export-NAVAppTenantWebService.md)
Exports the specified web service from a Dynamics NAV database to a file.

### [Get-NAVAppManifest](Get-NAVAppManifest.md)
Loads a manifest for an NAV App from an external source.

### [New-NAVAppManifest](New-NAVAppManifest.md)
Creates a new in-memory manifest object with the specified NAV App metadata.

### [New-NAVAppManifestFile](New-NAVAppManifestFile.md)
Creates a file with metadata for a NAV App package.

### [New-NAVAppPackage](New-NAVAppPackage.md)
Creates a NAV App package file (.navx) at the specified location based on the specified manifest file and source files.

### [Set-NAVAppManifest](Set-NAVAppManifest.md)
Sets one or more available properties on an in-memory manifest.