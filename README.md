+import {MDXProvider} from '@mdx-js/react'
 import {createRoot} from 'react-dom/client'
 import {Heading, /* … */ Table} from './components/index.js'
 import Post from './post.mdx' // Assumes an integration is used to compile MDX -> JS.
<p style="color:#82071e">@@ -13,4 +14,8 @@ const components = {</p>

 const container = document.getElementById('root')
 if (!container) throw new Error('Expected `root`')
 const root = createRoot(container)
-root.render(<Post components={components} />)
+root.render(
+  <MDXProvider components={components}>
+    <Post />
+  </MDXProvider>
+)
