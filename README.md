# unraid-templates

Unraid Docker templates for adiuv0's containers.

| Template | Image |
|---|---|
| [GameVault](templates/gamevault.xml) | `adiuv0/gamevault` |
| [events-dashboard](templates/events-dashboard.xml) | `adiuv0/events-dashboard` |

## Using these templates

In Unraid, go to Docker. At the bottom of the page, in **Template repositories**, add:

```
https://github.com/adiuv0/unraid-templates
```

Click Save. Then go to Docker → Add Container, open the **Template** dropdown, and pick the container.

To use a single template without adding the repository, copy its XML file to `/boot/config/plugins/dockerMan/templates-user/my-<name>.xml`.
