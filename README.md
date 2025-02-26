# Useful notes about New Relic

select filter(count(*), WHERE level = 'ERROR' AND  hostname = 'canary') / filter(count(*), where level = 'ERROR' OR level = 'INFO') FROM Log

percentage function:

SELECT percentage(count(*), WHERE level = 'INFO') as percent FROM Log SINCE 30 minutes ago <br/>
SELECT percentage(count(*), WHERE level = 'ERROR') as percent FROM Log SINCE 30 minutes ago
SELECT average(numeric(amount)) FROM Log SINCE 1740433906404 UNTIL 1740454301491
