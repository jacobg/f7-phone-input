# f7-phone-input

The purpose of this repository is to reproduce the following error that occurs when trying to use the vue-phone-number-input component:
```
vue.runtime.esm.js?2b0e:619 [Vue warn]: You may have an infinite update loop in a component render function.

found in

---> <CountrySelector> at CountrySelector.vue
       <VuePhoneNumberInput> at index.vue
         <F7PageContent>
           <F7Page>
             <PhonePage> at src/components/PhonePage.vue
               <F7View>
                 <F7App>
                   <App> at src/App.vue
                     <Root>
```

This error occurs when trying to open the country selector, or when filling in the national number input.

This error only happens when using f7 with webpack e6 modules. When using html and inline scripts, the error does not occur.

Here are demos of each:
1) webpack version - https://jacobg.github.io/f7-phone-input/index.html
2) inline version - https://jacobg.github.io/f7-phone-input/inline.html

