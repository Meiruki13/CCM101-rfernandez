# Reflection

Checking the host server's resources is important even when containers are
running perfectly, because the host is what every container ultimately
depends on. A container can be configured flawlessly and still fail if the
physical machine underneath it runs out of RAM or disk space — the
container has no way to perform better than the hardware hosting it
allows.

If a user complained they couldn't log in, the `docker logs` command would
let me see the exact HTTP requests hitting the server around the time of
the complaint. I could look for failed authentication attempts, 500-level
server errors, or requests that never completed, which would point
directly at whether the problem was on the client side, the network, or
the application itself.

The difference between monitoring logs and monitoring metrics is what
each one tells you. Logs (Checkpoint 4) are detailed, timestamped records
of individual events — they tell you *why* something happened. Metrics
(Checkpoint 5) are numerical measurements like CPU percentage and memory
usage sampled over time — they tell you *that* something is happening
right now. Monitoring alerts you there's a problem; logs let you
investigate the cause.

Large enterprise companies monitoring thousands of containers rely on
centralized tools rather than checking each one manually. A tool like
Prometheus pulls metrics from every server and container at regular
intervals and stores them in a time-series database, while Grafana turns
that data into dashboards engineers can scan at a glance — this scales to
fleets of machines in a way that running `docker stats` one container at a
time never could.

My ability to troubleshoot Linux environments has improved noticeably
since this lab. Instead of assuming a problem based on symptoms alone, I
now instinctively reach for the actual data — checking resource usage with
`free`, `df`, and `top`, and cross-referencing that against container logs
and live metrics — before drawing any conclusions about what's actually
wrong.
