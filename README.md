# unraid-templates

Unraid Docker templates for adiuv0's containers.

| Template | Image |
|---|---|
| [GameVault](templates/gamevault.xml) | `adiuv0/gamevault` |
| [events-dashboard](templates/events-dashboard.xml) | `adiuv0/events-dashboard` |

## Using these templates

Unraid 6.10 removed the Template repositories setting, and these templates aren't listed in Community Applications. To install one, copy its XML onto the flash drive. Open the Unraid terminal (the `>_` icon at the top right of the web UI) and run, for example:

```
wget -O /boot/config/plugins/dockerMan/templates-user/my-events-dashboard.xml \
  https://raw.githubusercontent.com/adiuv0/unraid-templates/main/templates/events-dashboard.xml
```

Then go to Docker → Add Container, open the **Template** dropdown, and pick the container under User templates.

Name the file `my-<Name>.xml`, where `<Name>` is the template's `<Name>` value (`my-GameVault.xml` for GameVault). Unraid saves your settings to that same file when you click Apply, so you get one entry in the dropdown instead of two.
