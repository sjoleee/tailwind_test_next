yarn berry에서 잘 되나?

tailwind config에 아래처럼 작성해주면 잘 됨.

```
import { dirname } from "path";

const packagePath = require.resolve("@sjoleee/tailwind-test-component");
const packageDir = dirname(packagePath);

content: [..., `${packageDir}/**/*.{js,ts,jsx,tsx}`]
```

yarn classic에서는??

```
content: [..., './node_modules/@sjoleee/tailwind-test-component/**/*.{js,ts,jsx,tsx}']

```
