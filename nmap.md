# nmap

A tool used for network discovery and port scanning.

## Useful Alias

See [.bash_aliases](./bash_aliases) for the following useful command:

```Shell
nmap -T4 -A -F -Pn {target}
```

This is the `nmap` scan that I default to when starting recon on a target.

Command breakdown:

| Switch | Description |
|--------|-------------|
| -T4 | -T4 does the equivalent of --max-rtt-timeout 1250ms --min-rtt-timeout 100ms --initial-rtt-timeout 500ms --max-retries 6 and sets the maximum TCP scan delay to 10 milliseconds. |
| -A | Enable OS detection, version detection, script scanning, and traceroute. |
| -F | Fast mode - Scan fewer ports than the default scanTreat all hosts as online -- skip host discovery. |
| -Pn | Treat all hosts as online -- skip host discovery. |
