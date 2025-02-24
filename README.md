# Useful notes about New Relic

select filter(count(*), WHERE level = 'ERROR' AND  hostname = 'canary') / filter(count(*), where level = 'ERROR' OR level = 'INFO') FROM Log
