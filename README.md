# kibana-vis-dropdown

A dropdown visualization which allows users to set filters from a list of values.

<img src="https://user-images.githubusercontent.com/10326954/30762662-29f25702-9fe3-11e7-9134-5aefbb1fb51c.png" width="350"/>

## Installation
To install the plugin, follow these steps...

1. Execute the following commands on the Kibana server.

```
> cd KIBANA_HOME/plugins
> git clone https://github.com/robcowart/kibana-vis-dropdown.git
> cd kibana-vis-dropdown
> npm install
```

2. Edit `package.json` setting the kibana version to the version of Kibana that is installed. Versions 5.5.x and 5.6.x should work.

```
kibana": {
  "version": "5.6.1"
},
```

3. Start Kibana.

```
> KIBANA_HOME/bin/kibana
```

## Configuration
To set up the dropdown visualization, create a Visualisation of type 'Dropdown Picker'

<img src="https://user-images.githubusercontent.com/10326954/30762214-51742e24-9fe1-11e7-9d53-444367a29cd1.png" width="150"/>

To configure the vizualization, leave the metric as count and click on `Field to filter on`. 

<img src="https://user-images.githubusercontent.com/10326954/30762756-87df1e5e-9fe3-11e7-8107-bbaa67587133.png" width="320"/>

Select the field from which to derive the values to be added to the dropdown list, the sort order and the maximum number of values to be listed.

<img src="https://user-images.githubusercontent.com/10326954/30762879-12e5b710-9fe4-11e7-8c9b-94612644a264.png" width="320"/>

In the visualisation options, you can set whether the dropdown is allowed to be blank. If this is true, you can hit escape while the dropdown is open to close it without selecting a value.

<img src="https://user-images.githubusercontent.com/10326954/30762941-5fad76e6-9fe4-11e7-9743-98347d475946.png" width="320"/>

Save the visualization and it can then be added to a dashboard, where it will be used to set filters by selecting an item from the dropdown list.
