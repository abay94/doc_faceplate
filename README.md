# Work With Grid Element

Grid element is documented well with demos in [Kendo UI](https://demos.telerik.com/kendo-ui/grid/index). In faceplate we can use it in the following manner:

> 1. Use in mnemonics
> 2. Use in (Отчеты)

As datasource we can use dynamic and static data, which can be added by Table datasource, TimeSeries data and JSON datasource.

## Let's configure grid with dynamic datasource

As an example, we will show a list of cars, with related dynamic and static paramaters, correspondingly for each car. As an output, we will end up with a table with Header names of : **Name , Brand, Color, Max Speed, Torque, Speed**

### All steps

> Firstly create a folder 

<img src="/img/1.png" width="350" height="250">

> Create tags for each car, and as for tag pattern (шаблон), it needs to create a new one. So let's create a tag pattern, for > that we click editor to choose a patterns (there are two option : *tags, patterns*)

<img src="/img/0_1.png" width="350" height="250">

> Then we will create a new pattern in our case *car* which has parameters of *Name , Brand, Color, Max Speed, Torque, Speed* > as we have mentioned before.

<img src="/img/0_2.png" width="550" height="350">

> While we adding a field we have to write name of parameter like "Brand" and type "string" and  storage type "ramdisc". 
> The  reason of choosing between ramdisc or ram depends on how the value of parameter needs to be 
> saved in hard disc. For example the parameter Name is not changed by the time more frequently and needs to be saved in disc
> but the parameter of "Speed" is changed everytime.
> So our pattern "car" will look like this:

<img src="/img/0_3.png" width="650" height="450">




