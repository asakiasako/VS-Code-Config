1. Install plugins

2. Edit config files: user settings, workspace settings, launch settings, keyboard shortcuts.

3. TS Types:
 
    * `package.json`: vue version = ^2.5.3 (or later)
   
    * Install type declarations if needed. For example, in devDependencies: 

        ``` json
        {
            "@types/lodash": "^4.14.77"
        }
        ```

    * Extend types to work with plugins. Make a `my-property.d.ts` file and put it into project.

        ``` js
        import Vue from 'vue'
        declare module 'vue/types/vue' {
            interface Vue {
                $myProperty: string
            }
        }
        ```
    
    * Official support for element-ui. If you install it in `dependency`, vue.js will load its tabs and props automatically.

4. Common keyboard shortcuts

    Some shortcuts already defined in config files for example. You can add new shortcuts with [Cmd+K Cmd+S] for mac. (For windows, use Ctrl instead of Cmd)