# NLMLab connection setup

NLMLab reads the live Non League Manager interface running on your own Windows PC through a local WebView2 debugging connection.

## Automatic setup

From **v1.5.1 Beta 2**, the NLMLab installer configures the required NLM connection automatically. You do **not** need to run a separate `.cmd` or PowerShell setup file.

### First install

1. Close Non League Manager completely.
2. Run the NLMLab installer.
3. Approve the Windows administrator prompt if it appears.
4. Start NLM normally through Steam.
5. Load your career.
6. Start NLMLab.

NLMLab should report **Connected to NLM**.

If NLM was already open during installation, close it completely and start it again once so the setting takes effect.

## What the installer changes

The installer adds a machine-level WebView2 browser argument for `nlfm.exe` so its local debugging endpoint is available on port **9222** while NLM is running. NLMLab reads that endpoint from the same PC.

This does not edit your NLM save or player data.

## Troubleshooting

If NLMLab does not connect:

- make sure NLM is running
- make sure a career is loaded
- if NLM was open during installation, close it fully and reopen it
- check that another application is not already using local port 9222
- retry the connection from NLMLab

When reporting a connection issue, include your NLMLab version, NLM version and a screenshot of the connection message.

## Removing the connection setting manually

If you later want to remove the WebView2 setting, close NLM and run PowerShell **as Administrator**:

```powershell
Remove-ItemProperty `
  -Path "HKLM:\Software\Policies\Microsoft\Edge\WebView2\AdditionalBrowserArguments" `
  -Name "nlfm.exe"
```

Then restart NLM. NLMLab will no longer be able to connect until the setting is enabled again.
