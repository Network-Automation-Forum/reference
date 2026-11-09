# Tools

Tools and utilities related to the NAF Framework. This section lists software, scripts, and other resources that can help with network automation using the NAF Framework.

<!-- Entries are ordered newest-first by date. -->

## Tools & Utilities

### NAF app map

**Owner:** Bart Dorlandt · [Source](https://github.com/bartdorlandt/naf_app_map)

Visualizes the network automation applications in their respective building blocks. Service runs locally.

![NAF app map overview](https://github.com/bartdorlandt/naf_app_map/blob/main/images/overview.png?raw=true){ width="600" }


### How Network Automation Works

**Owner:** Brian Jeggesen · [Website](https://hownetworkautomationworks.com/)

Interactive walkthrough of a network automation scenario (provision, detect, remediate) across the NAF Framework blocks, with simple and technical views.

![How Network Automation Works overview](https://hownetworkautomationworks.com/og.png){ width="600" }

## How to add an entry

1. If you have a tool or utility to host in the repo, drop the file into `docs/Framework/tools/` using an appropriate naming convention. External links are also fine — no file needed.
2. Add a section under **Tools & Utilities**, keeping entries ordered newest-first by date. Copy this template:

    ```markdown
    ### Tool name

    **Owner:** Your Name · [GitHub](https://github.com/…)

    Short description of what the tool does.

    ![Tool name screenshot](https://…/image.png){ width="600" }
    ```

3. Required fields: **Name** (the heading), **Owner**, and a description. The image is optional.
4. Open a pull request.

The links accept any combination of:

- `[Source](https://github.com/…)` — link to the source/repository
- `[Website](https://…)` — link to the project's website or documentation
- `[Download](tools/file)` — in-repo downloadable file
