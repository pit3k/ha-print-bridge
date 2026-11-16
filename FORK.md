# pit3k fork of Print Bridge

This is Piotr Paczyński's fork of [rubeecube/ha-print-bridge](https://github.com/rubeecube/ha-print-bridge), for installation through the Home Assistant Marketplace.

It includes a Direct IPP reachability probe: some printers (for example those using the Brother debut/1.30 HTTP server) close HTTP HEAD on the IPP endpoint, so setup and the online check use IPP Get-Printer-Attributes instead. The probe lives in `ipp_client.py` and shares the IPP POST path with Print-Job and the capabilities query.

- Upstream-PR branch (version left at 0.1.33): [`fix/ipp-probe-get-printer-attributes`](https://github.com/pit3k/ha-print-bridge/tree/fix/ipp-probe-get-printer-attributes)
- This release branch: [`pit3k`](https://github.com/pit3k/ha-print-bridge/tree/pit3k), version **0.1.33.2**

Do not open the `pit3k` branch as the upstream pull request.

Install in Home Assistant via **Settings → Marketplace → Add from link**: `https://github.com/pit3k/ha-print-bridge`.
