# Pricing model

## On Demand
you pay by the hour or the second,
depending on the type of instance you're running

## Reserved
you can reserve EC2 capacity for either one or three
years. you get up to a 72% discount on the hourly charge and
reserved instances operate at a **regional** level. **NOT cross region**.

 - Predicatble usage
 - Specific requirements
 - Pay upfront
 ### Reserved types
  
  - Standard Reserved Instances (RIs) - Upto 72% off on-demand price not convertible (Can not change the instance type from micro to large)
  - Convertible RIs - Upto 54% off on-demand price - has the option to change to a different reserved instance type of equal or greater value (T3.Large to T3.Extra large)
  - Scheduled RIs - launch a reserved instance within a time frame that
                    you specify and this allows you to match your capacity reservation
                    to a predictable recurring schedule,
                    which only requires either a fraction of a day, week, or month.

## Spot Instances
Purchase unused capacity at a massive discount of up to 90% and the price fluctuates according to
supply and demand. So you set a maximum price that you're willing to pay for the instance, but the catch is that as soon as the price exceeds your maximum,
the instance will be terminated or hibernated depending on the options that you've chosen. So you get a massive discount,
but it's not really suitable for every application.

- work really well for applications that are really only feasible at
very low compute prices.
 - suitable for applications or users with an urgent
need for large amounts of additional computing capacity,
which is temporary. So it's not an ongoing requirement,
it's just for a specific job or workload.
So you might use it spot instances for workloads like image rendering

## Dedicated
physical server running EC2 instances,
and it's dedicated for your use,
and it's actually the most expensive option, but it's a good option.
If you have software licenses, which are tied to physical hardware,
or if you have very strict compliance requirements,
which state that you cannot use multitenant hardware for your application.