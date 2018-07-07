# my-vue-autocomplete
a simple component with autocomplete input
Based in [this](http://fareez.info/blog/vuejs/create-your-own-autocomplete-using-vuejs-2/) article.


I just added some personal changes to display the list of suggestions by i/o of the input focus too.

## Usage
#### template
```html
<template>      
  <autocomplete 
    :suggestions="suggestions"
    v-model="selection">
  </autocomplete>
</template>
```

and the script shoud be
#### script
```html
<script>
import autocomplete from '@/components/Autocomplete'
export default {
    name: 'mycomponent',
    data () {
        return {    
          selection: '',
          suggestions: [
            {
              title:'OPTION',
              subtitle: 'description of the option'
            }
          ]
        }
    },
    components: {
      autocomplete
    }

}
</script>
```

The suggestions is an array of objects containing title and subtitle elements each.
:octocat:
