Steps:

- Make a new project with `lein new re-frame brokennav +10x +cider +routes`
- cd inside, `npm install`, `npm run watch`
- wait...
- open localhost:8280
- click on the links, they work
- open `src/brokennav/events.cljs`
- add an empty line with a comment ";"
- save it, browser hot reloads
- the links don't work anymore

```
sose@delli Linux 5.10.36-2-MANJARO x86_64 21.0.5 Ornara
~ >>> cd koodi/tmp                        
~/koodi/tmp >>> ls     
ajkstack  count.py  haskell-mooc  libraryof  my-app
~/koodi/tmp >>> lein new re-frame brokennav +10x +cider +routes                           
Generating re-frame project.
~/koodi/tmp >>> cd brokennav      
~/.../tmp/brokennav >>> npm install              

added 96 packages, and audited 97 packages in 5s

3 packages are looking for funding
  run `npm fund` for details

found 0 vulnerabilities
~/.../tmp/brokennav >>> npm run watch     

> watch
> npx shadow-cljs watch app browser-test karma-test

shadow-cljs - config: /home/sose/koodi/tmp/brokennav/shadow-cljs.edn
shadow-cljs - updating dependencies
shadow-cljs - dependencies updated
running: npm install --save --save-exact highlight.js@10.7.1 react@17.0.1 react-dom@17.0.1

added 6 packages, and audited 103 packages in 4s

3 packages are looking for funding
  run `npm fund` for details

found 0 vulnerabilities
No config for build "browser-test" found.
No config for build "karma-test" found.
shadow-cljs - HTTP server available at http://localhost:8280
shadow-cljs - HTTP server available at http://localhost:8290
shadow-cljs - server version: 2.12.5 running at http://localhost:9630
shadow-cljs - nREPL server started on port 8777
shadow-cljs - watching build :app
[:app] Configuring build.
[:app] Compiling ...
------ WARNING #1 -  -----------------------------------------------------------
 Resource: node_modules/highlight_DOT_js/lib/core.js:1475:23
 Missing "..." in type annotation for rest parameter.
--------------------------------------------------------------------------------
[:app] Build completed. (551 files, 550 compiled, 0 warnings, 69.00s)
[:app] Compiling ...
[:app] Build completed. (551 files, 4 compiled, 0 warnings, 0.95s)
```