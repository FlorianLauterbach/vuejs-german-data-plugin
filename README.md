# vuejs-german-data-plugin
A small plugin for german cities, districts and states


## installation
add Germany.js file to your project and be careful. This file is not a lightweight - if you're using it within a webapp, you should reduce the data to a minimum :) 

install the file in your ``main.js`` file

~~~ 
import { createApp } from  'vue'
import App from  './App.vue'
import { GermanData } from  './plugins/Germany.js'

const app = createApp(App).use(GermanData)

router.isReady().then(() => {
	app.mount('#app');
});
~~~

now you have global access to the following data:
``this.$germanData`` - the whole array of objects

``this.$getStates()`` - get all states

``this.$getDistrictByState(state)``- get all districts by state name parameter

``this.$getAllDistricts()``- get all districts

``this.$getCitiesByDistrict(disctrict)`` - get alls cities by state name parameter
