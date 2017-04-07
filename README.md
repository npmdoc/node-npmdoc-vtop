# api documentation for  [vtop (v0.5.7)](http://parall.ax/vtop)  [![npm package](https://img.shields.io/npm/v/npmdoc-vtop.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-vtop) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-vtop.svg)](https://travis-ci.org/npmdoc/node-npmdoc-vtop)
#### Wow such top. So stats

[![NPM](https://nodei.co/npm/vtop.png?downloads=true)](https://www.npmjs.com/package/vtop)

[![apidoc](https://npmdoc.github.io/node-npmdoc-vtop/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-vtop_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-vtop/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-vtop/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-vtop/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "James Hall",
        "email": "james@parall.ax"
    },
    "bin": {
        "vtop": "./bin/vtop.js"
    },
    "bugs": {
        "url": "https://github.com/MrRio/vtop/issues"
    },
    "dependencies": {
        "blessed": "0.1.81",
        "commander": "2.7.1",
        "drawille": "1.0.0",
        "glob": "5.0.2",
        "husky": "^0.11.9",
        "os-utils": "0.0.14",
        "read": "1.0.5",
        "safe-eval": "^0.3.0",
        "sudo": "1.0.3",
        "use-strict": "^1.0.1"
    },
    "description": "Wow such top. So stats",
    "devDependencies": {},
    "directories": {},
    "dist": {
        "shasum": "fff91000fac3a97a165f6f52dc253bce3d4d091e",
        "tarball": "https://registry.npmjs.org/vtop/-/vtop-0.5.7.tgz"
    },
    "engines": {
        "node": ">=0.10.0"
    },
    "gitHead": "182990627cf9ce89368de5baad786e16d5a0c974",
    "homepage": "http://parall.ax/vtop",
    "license": "MIT",
    "main": "app.js",
    "maintainers": [
        {
            "name": "mrjameshall",
            "email": "james@parall.ax"
        }
    ],
    "name": "vtop",
    "optionalDependencies": {},
    "preferGlobal": true,
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git+ssh://git@github.com/MrRio/vtop.git"
    },
    "scripts": {
        "precommit": "standard",
        "test": "make test"
    },
    "standard": {
        "ignore": [
            "bin/vtop.js"
        ]
    },
    "version": "0.5.7"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module vtop](#apidoc.module.vtop)
1.  object <span class="apidocSignatureSpan">vtop.</span>cpu
1.  object <span class="apidocSignatureSpan">vtop.</span>memory
1.  object <span class="apidocSignatureSpan">vtop.</span>process
1.  object <span class="apidocSignatureSpan">vtop.</span>upgrade

#### [module vtop.cpu](#apidoc.module.vtop.cpu)
1.  boolean <span class="apidocSignatureSpan">vtop.cpu.</span>initialized
1.  [function <span class="apidocSignatureSpan">vtop.cpu.</span>poll ()](#apidoc.element.vtop.cpu.poll)
1.  number <span class="apidocSignatureSpan">vtop.cpu.</span>currentValue
1.  number <span class="apidocSignatureSpan">vtop.cpu.</span>interval
1.  string <span class="apidocSignatureSpan">vtop.cpu.</span>title
1.  string <span class="apidocSignatureSpan">vtop.cpu.</span>type

#### [module vtop.memory](#apidoc.module.vtop.memory)
1.  boolean <span class="apidocSignatureSpan">vtop.memory.</span>initialized
1.  boolean <span class="apidocSignatureSpan">vtop.memory.</span>isLinux
1.  [function <span class="apidocSignatureSpan">vtop.memory.</span>poll ()](#apidoc.element.vtop.memory.poll)
1.  number <span class="apidocSignatureSpan">vtop.memory.</span>currentValue
1.  number <span class="apidocSignatureSpan">vtop.memory.</span>interval
1.  string <span class="apidocSignatureSpan">vtop.memory.</span>title
1.  string <span class="apidocSignatureSpan">vtop.memory.</span>type

#### [module vtop.process](#apidoc.module.vtop.process)
1.  boolean <span class="apidocSignatureSpan">vtop.process.</span>initialized
1.  [function <span class="apidocSignatureSpan">vtop.process.</span>poll ()](#apidoc.element.vtop.process.poll)
1.  number <span class="apidocSignatureSpan">vtop.process.</span>interval
1.  object <span class="apidocSignatureSpan">vtop.process.</span>columns
1.  object <span class="apidocSignatureSpan">vtop.process.</span>currentValue
1.  string <span class="apidocSignatureSpan">vtop.process.</span>description
1.  string <span class="apidocSignatureSpan">vtop.process.</span>sort
1.  string <span class="apidocSignatureSpan">vtop.process.</span>title
1.  string <span class="apidocSignatureSpan">vtop.process.</span>type

#### [module vtop.upgrade](#apidoc.module.vtop.upgrade)
1.  [function <span class="apidocSignatureSpan">vtop.upgrade.</span>check (callback)](#apidoc.element.vtop.upgrade.check)
1.  [function <span class="apidocSignatureSpan">vtop.upgrade.</span>install (packageName, vars)](#apidoc.element.vtop.upgrade.install)



# <a name="apidoc.module.vtop"></a>[module vtop](#apidoc.module.vtop)



# <a name="apidoc.module.vtop.cpu"></a>[module vtop.cpu](#apidoc.module.vtop.cpu)

#### <a name="apidoc.element.vtop.cpu.poll"></a>[function <span class="apidocSignatureSpan">vtop.cpu.</span>poll ()](#apidoc.element.vtop.cpu.poll)
- description and source-code
```javascript
poll() {
  os.cpuUsage(v => {
    plugin.currentValue = (Math.floor(v * 100))
    plugin.initialized = true
  })
}
```
- example usage
```shell
...
  selectedProcess = selectedProcess.slice(0, processWidth).trim()

  childProcess.exec('killall "${selectedProcess}"', () => {})
}

if (key.name === 'c' && charts[2].plugin.sort !== 'cpu') {
  charts[2].plugin.sort = 'cpu'
  charts[2].plugin.poll()
  setTimeout(() => {
    processListSelection.select(0)
  }, 200)
}
if (key.name === 'm' && charts[2].plugin.sort !== 'mem') {
  charts[2].plugin.sort = 'mem'
  charts[2].plugin.poll()
...
```



# <a name="apidoc.module.vtop.memory"></a>[module vtop.memory](#apidoc.module.vtop.memory)

#### <a name="apidoc.element.vtop.memory.poll"></a>[function <span class="apidocSignatureSpan">vtop.memory.</span>poll ()](#apidoc.element.vtop.memory.poll)
- description and source-code
```javascript
poll() {
  const computeUsage = (used, total) => Math.round(100 * (used / total))

  if (plugin.isLinux) {
    child.exec('free -m', (err, stdout, stderr) => {
      if (err) {
        console.error(err)
      }
      const data = stdout.split('\n')[1].replace(/[\s\n\r]+/g, ' ').split(' ')
      const used = parseInt(data[2], 10)
      const total = parseInt(data[1], 10)
      plugin.currentValue = computeUsage(used, total)
    })
  } else {
    plugin.currentValue = Math.round((1 - os.freememPercentage()) * 100)
  }

  plugin.initialized = true
}
```
- example usage
```shell
...
  selectedProcess = selectedProcess.slice(0, processWidth).trim()

  childProcess.exec('killall "${selectedProcess}"', () => {})
}

if (key.name === 'c' && charts[2].plugin.sort !== 'cpu') {
  charts[2].plugin.sort = 'cpu'
  charts[2].plugin.poll()
  setTimeout(() => {
    processListSelection.select(0)
  }, 200)
}
if (key.name === 'm' && charts[2].plugin.sort !== 'mem') {
  charts[2].plugin.sort = 'mem'
  charts[2].plugin.poll()
...
```



# <a name="apidoc.module.vtop.process"></a>[module vtop.process](#apidoc.module.vtop.process)

#### <a name="apidoc.element.vtop.process.poll"></a>[function <span class="apidocSignatureSpan">vtop.process.</span>poll ()](#apidoc.element.vtop.process.poll)
- description and source-code
```javascript
poll() {
  const stats = {}
  // @todo If you can think of a better way of getting process stats,
  // then please feel free to send me a pull request. This is version 0.1
  // and needs some love.
  childProcess.exec('ps -ewwwo %cpu,%mem,comm', (error, stdout, stderr) => {
    if (error) {
      console.error(error)
    }
    const lines = stdout.split('\n')
    // Ditch the first line
    lines[0] = ''
    for (const line in lines) {
      const currentLine = lines[line].trim().replace('  ', ' ')
      const words = currentLine.split(' ')
      if (typeof words[0] !== 'undefined' && typeof words[1] !== 'undefined') {
        const cpu = words[0].replace(',', '.')
        const mem = words[1].replace(',', '.')
        const offset = cpu.length + mem.length + 2
        let comm = currentLine.slice(offset)
        // If we're on Mac then remove the path
        if (/^darwin/.test(process.platform)) {
          comm = comm.split('/')
          comm = comm[comm.length - 1]
        } else {
          // Otherwise assume linux and remove the unnecessary /1 info like
          // you get on kworker
          comm = comm.split('/')
          comm = comm[0]
        }
        // If already exists, then add them together
        if (typeof stats[comm] !== 'undefined') {
          stats[comm] = {
            cpu: parseFloat(stats[comm].cpu, 10) + parseFloat(cpu),
            mem: parseFloat(stats[comm].mem, 10) + parseFloat(mem),
            comm,
            count: parseInt(stats[comm].count, 10) + 1
          }
        } else {
          stats[comm] = {
            cpu,
            mem,
            comm,
            count: 1
          }
        }
      }
    }
    const statsArray = []
    for (const stat in stats) {
      // Divide by number of CPU cores
      const cpuRounded = parseFloat(stats[stat].cpu / os.cpus().length).toFixed(1)
      const memRounded = parseFloat(stats[stat].mem).toFixed(1)
      statsArray.push({
        'Command': stats[stat].comm,
        'Count': stats[stat].count,
        'CPU %': cpuRounded,
        'Memory %': memRounded,
        'cpu': stats[stat].cpu,
        'mem': stats[stat].mem // exact cpu for comparison
      })
    }
    statsArray.sort((a, b) => parseFloat(b[plugin.sort]) - parseFloat(a[plugin.sort]))

    plugin.currentValue = statsArray
    plugin.initialized = true
  })
}
```
- example usage
```shell
...
  selectedProcess = selectedProcess.slice(0, processWidth).trim()

  childProcess.exec('killall "${selectedProcess}"', () => {})
}

if (key.name === 'c' && charts[2].plugin.sort !== 'cpu') {
  charts[2].plugin.sort = 'cpu'
  charts[2].plugin.poll()
  setTimeout(() => {
    processListSelection.select(0)
  }, 200)
}
if (key.name === 'm' && charts[2].plugin.sort !== 'mem') {
  charts[2].plugin.sort = 'mem'
  charts[2].plugin.poll()
...
```



# <a name="apidoc.module.vtop.upgrade"></a>[module vtop.upgrade](#apidoc.module.vtop.upgrade)

#### <a name="apidoc.element.vtop.upgrade.check"></a>[function <span class="apidocSignatureSpan">vtop.upgrade.</span>check (callback)](#apidoc.element.vtop.upgrade.check)
- description and source-code
```javascript
check = function (callback) {
  try {
    var current = require('./package.json').version

    var childProcess = require('child_process')
    childProcess.exec('npm --color=false info vtop', function (error, stdout, stderr) {
      if (error) {
        console.error(error)
      }
      var output = safeEval('(' + stdout + ')')
      if (output['dist-tags']['latest'] !== current) {
        callback(output['dist-tags']['latest'])
      } else {
        callback(false)
      }
    })
  } catch (e) {
    callback(false)
  }
}
```
- example usage
```shell
...
// Create a screen object.
screen = blessed.screen()

// Configure 'q', esc, Ctrl+C for quit
let upgrading = false

const doCheck = () => {
  upgrade.check(v => {
    upgradeNotice = v
    drawHeader()
  })
}

doCheck()
// Check for updates every 5 minutes
...
```

#### <a name="apidoc.element.vtop.upgrade.install"></a>[function <span class="apidocSignatureSpan">vtop.upgrade.</span>install (packageName, vars)](#apidoc.element.vtop.upgrade.install)
- description and source-code
```javascript
install = function (packageName, vars) {
  var sudo = require('sudo')
  console.log('')
  console.log('Installing vtop update...')
  console.log('')
  console.log(' ** You will need to enter your password to upgrade ** ')
  console.log('')

  var args = ['npm', 'install', '-g', 'vtop']
  console.log(args.join(' '))

  var options = {
    cachePassword: false,
    prompt: 'Password:',
    spawnOptions: { stdio: 'inherit' }
  }
  var child = sudo(args, options)

  var path = false
  child.stdout.on('data', function (data) {
    console.log(data.toString())

    if (data.toString().indexOf('vtop.js') !== -1) {
      path = data.toString().trim().split(' ')[2]
    }
  })
  child.stderr.on('data', function (data) {
    console.log(data.toString())
  })

  child.on('close', function () {
    for (var file in require.cache) {
      delete require.cache[file]
    }
    console.log('Finished updating. Clearing cache and relaunching...')
    setTimeout(function () {
      for (var v in vars) {
        process[v] = vars[v]
      }
      require(path)
    }, 1000)
  })
}
```
- example usage
```shell
...
  program = blessed.program()
  program.clear()
  program.disableMouse()
  program.showCursor()
  program.normalBuffer()

  // @todo: show changelog  AND  smush existing data into it :D
  upgrade.install('vtop', [
    {
      'theme': theme
    }
  ])
}

if ((key.name === 'left' || key.name === 'h') && graphScale < 8) {
...
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
