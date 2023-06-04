# vuejs-german-data-plugin
An small plugin for german cities, districts and states


## installation
add Germany.js file to your project

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

``this.$getCitiesByDistrict(disctrict)`` - get alls cities by state name parameter
