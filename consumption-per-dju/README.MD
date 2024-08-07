# Report description

The report display a graph of the consumption per dju of the building. The graph is displayed in a line chart. The
x-axis represents the date and the y-axis represents the consumption per dju

# How to use

The integrator can copy the code and paste it in an advanced report in the advanced report section of the SCorp-io
designer platform.

As the macro contains the @STARTDATE@ and @ENDATE@ strings, the integrator must set the advanced report to display the
date selector and choose a duration.

Before saving the report; the integrator have to modify some constants in the macro code in order to adapt the report to
the building he wants to display the consumption per dju.

The constants are defined at the beginning of the macro tag ( 'macro' <% ) :

```
  /* CONSTANTS TO DEFINE BEGIN SECTION */
   'd7939c54-8608-4330-90c9-4cee7be655fa' 'projectId' STORE
   'PCE - GI 055241' 'objectInstanceName' STORE
   'GRDF' 'objectModelName' STORE
   'Energie quotidienne' 'attributeModelName' STORE
   /* CONSTANTS TO DEFINE END SECTION */
```

The integrator have to modify the following constants :

- 'projectId' : the projectId of SCorp-io project
- 'objectInstanceName' : the name of the object instance carrying the consumption variable
- 'attributeModelName' : the attribute model name of the consumption

Enjoy the report !