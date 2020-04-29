# Work With Grid Element

Grid element is documented well with demos in [Kendo UI](https://demos.telerik.com/kendo-ui/grid/index). In faceplate we can use it in the following manner:

> 1. Use in mnemonics
> 2. Use in (Отчеты)

As datasource we can use dynamic and static data, which can be added by Table datasource, TimeSeries data and JSON datasource.

## Let's configure grid with dynamic datasource

As an example, we will show a list of cars, with related dynamic and static paramaters, correspondingly for each car. As an output, we will end up with a table with Header names of : **Name , Brand, Color, Max_Speed, Torque, Speed**

### All steps

> Firstly create a folder 

<img src="/img/1.png" width="350" height="250">

> Create tags for each car, and as for tag pattern (шаблон), it needs to create a new one. So let's create a tag pattern, for > that we click editor to choose a patterns (there are two option : *tags, patterns*)

<kbd><img src="/img/0_1.png" width="550" height="250"></kbd>

> Then we will create a new pattern in our case *car* which has parameters of *NAME , Brand, Color, Max Speed, Torque, Speed*
> as we have mentioned before.

<img src="/img/0_2.png" width="650" height="350">

> While we adding a field we have to write name of parameter like "Brand" and type "string" and  storage type "ramdisc". 
> The  reason of choosing between ramdisc or ram depends on how the value of parameter needs to be 
> saved in hard disc. For example the parameter Name is not changed by the time more frequently and needs to be saved in disc
> but the parameter of "Speed" is changed everytime.
> So our pattern "car" will look like this:

<img src="/img/0_3.png" width="850" height="450">


> Then, we will create tags with pattern "car", what we have created.

<img src="/img/0_4.png" width="850" height="450">



> After that we will create (отчет)

<img src="/img/0_5.png" width="850" height="450">


> Then we will drang and drop elements of table datasource (TDS) and grid 

<img src="/img/0_6.png" width="850" height="450">


> By clicking twice on TDS, we can configure it, here we give a name for it


<img src="/img/0_7.png" width="850" height="450">


> The main configurations will be made here on data. Here we choosed "CAR" as source table, it means that this TDS can handle > all tags with pattern of "CAR" what we have created before.

<img src="/img/0_8.png" width="850" height="450">


> Not least and not last important configuration will be made in fields. Here, we shows which fields (parameters) will be used 
> in grid

<img src="/img/0_9.png" width="850" height="450">


> After that we can give a base filter as follows. Here, the json means that TDS will take only those tags with pattern of 
> "CAR" and direction of where it locates ".PATH:/root/PROJECT/TAGS/NEW BRANCH/Test for grid". Then compile and OK to save it.

<img src="/img/0_10.png" width="850" height="450">


> For option subscribe we choose "true" for dynamic changing each cells of grid.

<img src="/img/0_11.png" width="850" height="450">

> So let's start configuring a gtid. As it can be seen, here we firstly choose datasource "TDS_car" which we have created

<img src="/img/0_12.png" width="850" height="450">


> Then we choose JSON of config and edit it. The "field" value have to be the same as "fields" which are configured for TDS
> **NAME , Brand, Color, Max_Speed, Torque, Speed**. Then compile and OK to save it.

<img src="/img/0_13.png" width="850" height="450">


> Then we can see our grid (table with dynamic data) on runtime page


<img src="/img/0_14.png" width="850" height="450">


In order to make it more pretty, we can change and add some paramters in JSON of config, related to KENDO UI documentation.





