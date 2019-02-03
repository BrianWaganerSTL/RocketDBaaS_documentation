<h1>Tracking Issues</h1>

<h3>These are issues that if they cross thresholds we should alert in some manor</h3>

<table>
<tr><th>Tracker Issue</th><th>Warning</th><th>Critical</th></tr>
<tr><td>Server ping</td><td>>= 50ms or total failure</td><td>>= 100ms</td></tr>
<tr><td>DB connection time</td><td>>= 50ms or total failure</td><td>>= 100ms</td></tr>
<tr><td>MountPoint UsedPct</td><td>>= 80%</td><td>>= 95%</td></tr>
<tr><td>CPU load</td><td>>= 3 x Cpu Count</td><td>>= 10 x Cpu Count</td></tr>
<tr><td>CPU Idle Pct</td><td><= 10%</td><td></td></tr>
<tr><td>Cluster Health</td><td>Active Host < Hosts</td><td>Active Host <= 1</td></tr>
</tr>

All thresholds are setable.  Also how many ticks before we call it valid.
