### Inframer Analyzers

* Sample analyzers written on top of inframer API:
  - ips\_set\_operations: Perform set operations (whatever operations are provided by python's set module) on 2 inframer views
``` 
python ips_set_operations.py http://$INFRAMER_API_HOST:$INFRAMER_API_PORT/inframer/api/v1/db  aws/region/us-west-1 difference nagios/host_status
``` 
  - This will show you the set diff in the IPs between AWS region us-west-1 and your monitored nagios hosts i.e. which of my AWS us-west-1 region are not monitored
