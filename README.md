# Decentraland Skeleton Module

- Clone this repo to a local folder called **skeleton-module**.
- Run `npm link` in the folder.
- Create a new folder somewhere else called **master-project**
- In this new folder run `dcl init` to create a new empty project
- In this folder run `npm link skeleton-module`
- in **/src/game.ts** remove all the existing code and paste the following:

```
import { CustomUI } from '../node_modules/skeleton-module/src/customUI'

var customUI = new CustomUI()
customUI.ShowPrompt()
```

- Run the project with `dcl start`
- observe the error `Error: These modules didn't load: node_modules/skeleton-module/src/customUI, @dcl/ui-scene-utils, src/game`
