# vite-plugin-ftp
a simple useful vite ftp plugin, based on [ftp-deploy](https://github.com/simonh1000/ftp-deploy), upload your dist file after vite build.

# install
```
> npm i vite-plugin-ftp --save-dev
```

# usage

```js
// vite.config.ts
import vitePluginFtp from 'vite-plugin-ftp'

export default {
  plugins: [
    vitePluginFtp({
        host: '127.0.0.1',
        port: 21,
        remoteDir: '/www/wwwroot',
        user: 'root',
        password: '123456',
    })
  ]
}
```