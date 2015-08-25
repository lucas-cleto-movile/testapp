# testapp logs

```
$ java -version
java version "1.7.0_75"
Java(TM) SE Runtime Environment (build 1.7.0_75-b13)
Java HotSpot(TM) 64-Bit Server VM (build 24.75-b04, mixed mode)
```

```
$ lein -version
Leiningen 2.5.2 on Java 1.7.0_75 Java HotSpot(TM) 64-Bit Server VM
```

```
$ cat ~/.lein/profiles.clj
{:user {:plugins [[cider/cider-nrepl "0.10.0-SNAPSHOT"] [lein-droid "0.4.0-alpha4"]]
        :dependencies [[org.clojure/tools.nrepl "0.2.7"]]}
 :android-user {:plugins [[cider/cider-nrepl "0.10.0-SNAPSHOT"] [lein-droid "0.4.0-alpha4"]]
                :dependencies [[cider/cider-nrepl "0.9.1"]]
                :android {:aot-exclude-ns ["cider.nrepl.middleware.util.java.parser"
                                           "cider.nrepl" "cider-nrepl.plugin"]}}}
```

```
$ lein new droid testapp com.test.testapp :target-sdk 23
Using lein-droid 0.4.1
```

```
$ lein droid doall
(Warning: profile :android-common not found.)
Generating manifest...
Generating R.java...
(Warning: profile :android-common not found.)
Compiling 2 source files to /Users/lucas-cleto/biometria/testapp/target/debug/classes
Compiling Clojure files...
Build type: debug, dynamic compilation: enabled, remote REPL: enabled.
Compiling mranderson045.toolsnamespace.v0v2v11.clojure.tools.namespace.file
Compiling clojure.zip
Compiling mranderson045.cljfmt.v0v3v0.rewrite-clj.v0v4v12.rewrite-clj.zip.find
Compiling neko.log
Compiling clojure.reflect
Compiling cider.nrepl.middleware.info
Compiling mranderson045.toolsreader.v0v9v2.clojure.tools.reader.edn
Compiling mranderson045.compliment.v0v2v5-20150718v212238-1.compliment.sources.resources
Compiling cider.nrepl.middleware.inspect
Compiling clojure.tools.nrepl.middleware.pr-values
Compiling clojure.stacktrace
Compiling mranderson045.cljfmt.v0v3v0.rewrite-clj.v0v4v12.rewrite-clj.node.whitespace
Compiling mranderson045.cljfmt.v0v3v0.rewrite-clj.v0v4v12.rewrite-clj.parser.keyword
Compiling cider.nrepl.middleware.debug
Compiling cider.nrepl.middleware.stacktrace
Compiling mranderson045.cljfmt.v0v3v0.rewrite-clj.v0v4v12.rewrite-clj.parser.string
Compiling cider.nrepl.middleware.test
Compiling clojure.tools.nrepl.middleware.load-file
Compiling clojure.pprint
Compiling cider.nrepl.middleware.util.misc
Compiling clojure.tools.nrepl.cmdline
Compiling neko.intent
Compiling mranderson045.cljfmt.v0v3v0.rewrite-clj.v0v4v12.rewrite-clj.parser.core
Compiling mranderson045.cljs-tooling.v0v1v7.cljs-tooling.complete
Compiling clojure.java.io
Compiling clojure.main
Compiling mranderson045.compliment.v0v2v5-20150718v212238-1.compliment.sources.namespaces-and-classes
Compiling neko.data.sqlite
Compiling mranderson045.toolsnamespace.v0v2v11.clojure.tools.namespace.parse
Compiling clojure.tools.nrepl.server
Compiling mranderson045.cljfmt.v0v3v0.rewrite-clj.v0v4v12.rewrite-clj.parser.utils
Compiling mranderson045.toolsnamespace.v0v2v11.clojure.tools.namespace.find
Compiling neko.listeners.adapter-view
Compiling clojure.set
Compiling mranderson045.cljs-tooling.v0v1v7.cljs-tooling.info
Compiling mranderson045.toolsnamespace.v0v2v11.clojure.tools.namespace.track
Compiling neko.data.shared-prefs
Compiling mranderson045.toolsnamespace.v0v2v11.clojure.tools.namespace
Compiling mranderson045.toolsnamespace.v0v2v11.clojure.tools.namespace.move
Compiling mranderson045.compliment.v0v2v5-20150718v212238-1.compliment.sources.local-bindings
Compiling neko.context
Compiling dynapath.dynamic-classpath
Compiling mranderson045.cljfmt.v0v3v0.rewrite-clj.v0v4v12.rewrite-clj.node.protocols
Compiling com.test.testapp.main
Compiling mranderson045.compliment.v0v2v5-20150718v212238-1.compliment.sources.class-members
Compiling neko.ui.adapters
Compiling clojure.core
Compiling cider.nrepl.middleware.complete
Compiling mranderson045.compliment.v0v2v5-20150718v212238-1.compliment.utils
Compiling mranderson045.compliment.v0v2v5-20150718v212238-1.defprecated.v0v1v2.defprecated.core
Compiling neko.data
Compiling clojure.core.protocols
Compiling clojure.test.junit
Compiling neko.notify
Compiling neko.resource
Compiling mranderson045.compliment.v0v2v5-20150718v212238-1.compliment.sources.keywords
Compiling clojure.tools.nrepl
Compiling mranderson045.cljs-tooling.v0v1v7.cljs-tooling.util.misc
Compiling mranderson045.toolsreader.v0v9v2.clojure.tools.reader.impl.ExceptionInfo
Compiling mranderson045.cljfmt.v0v3v0.rewrite-clj.v0v4v12.rewrite-clj.zip
Compiling neko.compliment.ui-widgets-and-attributes
Compiling mranderson045.toolsreader.v0v9v2.clojure.tools.reader
Compiling clojure.tools.nrepl.bencode
Compiling mranderson045.cljfmt.v0v3v0.rewrite-clj.v0v4v12.rewrite-clj.parser.whitespace
Compiling mranderson045.toolsreader.v0v9v2.clojure.tools.reader.impl.commons
Compiling clojure.walk
Compiling mranderson045.cljfmt.v0v3v0.rewrite-clj.v0v4v12.rewrite-clj.node.meta
Compiling neko.listeners.dialog
Compiling mranderson045.compliment.v0v2v5-20150718v212238-1.compliment.sources.ns-mappings
Compiling clojure.edn
Compiling neko.debug
Compiling mranderson045.toolsnamespace.v0v2v11.clojure.tools.namespace.dir
Compiling neko.threading
Compiling cider.nrepl.middleware.refresh
Compiling dynapath.util
Compiling neko.listeners.text-view
Compiling cider.nrepl.middleware.trace
Compiling mranderson045.cljfmt.v0v3v0.rewrite-clj.v0v4v12.rewrite-clj.potemkin
Compiling clojure.tools.nrepl.middleware
Compiling mranderson045.javaclasspath.v0v2v2.clojure.java.classpath
Compiling mranderson045.cljfmt.v0v3v0.rewrite-clj.v0v4v12.rewrite-clj.zip.edit
Compiling clojure.test
Compiling clojure.java.shell
Compiling neko.listeners.view
Compiling cider.nrepl.middleware.undef
Compiling mranderson045.compliment.v0v2v5-20150718v212238-1.compliment.core
Compiling mranderson045.cljfmt.v0v3v0.rewrite-clj.v0v4v12.rewrite-clj.node.coerce
Compiling mranderson045.cljfmt.v0v3v0.rewrite-clj.v0v4v12.rewrite-clj.node
Compiling neko.tools.repl
Compiling mranderson045.toolsnamespace.v0v2v11.clojure.tools.namespace.dependency
Compiling neko.dialog.alert
Compiling mranderson045.cljfmt.v0v3v0.rewrite-clj.v0v4v12.rewrite-clj.node.forms
Compiling clojure.instant
Compiling mranderson045.toolsreader.v0v9v2.clojure.tools.reader.impl.utils
Compiling clojure.xml
Compiling neko.ui
Compiling cider.nrepl.middleware.util.instrument
Compiling neko.ui.listview
Compiling mranderson045.cljfmt.v0v3v0.rewrite-clj.v0v4v12.rewrite-clj.zip.base
Compiling clojure.string
Compiling mranderson045.cljfmt.v0v3v0.rewrite-clj.v0v4v12.rewrite-clj.node.uneval
Compiling clojure.uuid
Compiling mranderson045.toolsreader.v0v9v2.clojure.tools.reader.default-data-readers
Compiling mranderson045.toolsnamespace.v0v2v11.clojure.tools.namespace.repl
Compiling mranderson045.cljfmt.v0v3v0.rewrite-clj.v0v4v12.rewrite-clj.parser.token
Compiling cider.nrepl.middleware.util.java
Compiling cider.nrepl.middleware.classpath
Compiling neko.listeners.search-view
Compiling cider.nrepl.middleware.macroexpand
Compiling mranderson045.toolsreader.v0v9v2.clojure.tools.reader.reader-types
Compiling clojure.tools.nrepl.ack
Compiling mranderson045.cljfmt.v0v3v0.rewrite-clj.v0v4v12.rewrite-clj.node.keyword
Compiling clojure.tools.nrepl.helpers
Compiling mranderson045.compliment.v0v2v5-20150718v212238-1.compliment.sources
Compiling mranderson045.cljfmt.v0v3v0.rewrite-clj.v0v4v12.rewrite-clj.zip.remove
Compiling neko.activity
Compiling neko.find-view
Compiling clojure.template
Compiling mranderson045.compliment.v0v2v5-20150718v212238-1.compliment.sources.special-forms
Compiling mranderson045.cljfmt.v0v3v0.rewrite-clj.v0v4v12.rewrite-clj.node.integer
Compiling mranderson045.cljfmt.v0v3v0.rewrite-clj.v0v4v12.rewrite-clj.node.seq
Compiling clojure.tools.nrepl.middleware.session
Compiling mranderson045.cljfmt.v0v3v0.rewrite-clj.v0v4v12.rewrite-clj.node.comment
Compiling neko.action-bar
Compiling mranderson045.toolstrace.v0v7v8.clojure.tools.trace
Compiling mranderson045.cljfmt.v0v3v0.rewrite-clj.v0v4v12.rewrite-clj.zip.seq
Compiling cider.nrepl.middleware.util.cljs
Compiling dynapath.defaults
Compiling cider.nrepl.middleware.resource
Compiling cider.nrepl.middleware.ns
Compiling mranderson045.cljfmt.v0v3v0.rewrite-clj.v0v4v12.rewrite-clj.node.quote
Compiling mranderson045.cljfmt.v0v3v0.rewrite-clj.v0v4v12.rewrite-clj.node.indent
Compiling cider.nrepl.version
Compiling mranderson045.cljfmt.v0v3v0.rewrite-clj.v0v4v12.rewrite-clj.node.reader-macro
Compiling cider.nrepl.middleware.format
Compiling mranderson045.cljfmt.v0v3v0.rewrite-clj.v0v4v12.rewrite-clj.zip.utils
Compiling mranderson045.cljfmt.v0v3v0.rewrite-clj.v0v4v12.rewrite-clj.zip.move
Compiling mranderson045.cljfmt.v0v3v0.rewrite-clj.v0v4v12.rewrite-clj.zip.whitespace
Compiling clojure.tools.nrepl.misc
Compiling mranderson045.compliment.v0v2v5-20150718v212238-1.compliment.context
Compiling mranderson045.cljfmt.v0v3v0.rewrite-clj.v0v4v12.rewrite-clj.reader
Compiling mranderson045.cljfmt.v0v3v0.cljfmt.core
Compiling neko.ui.traits
Compiling mranderson045.cljfmt.v0v3v0.rewrite-clj.v0v4v12.rewrite-clj.node.fn
Compiling mranderson045.cljfmt.v0v3v0.rewrite-clj.v0v4v12.rewrite-clj.zip.insert
Compiling mranderson045.cljfmt.v0v3v0.rewrite-clj.v0v4v12.rewrite-clj.parser
Compiling neko.ui.menu
Compiling clojure.data
Compiling mranderson045.cljfmt.v0v3v0.rewrite-clj.v0v4v12.rewrite-clj.zip.subedit
Compiling neko.ui.mapping
Compiling mranderson045.toolsnamespace.v0v2v11.clojure.tools.namespace.reload
Compiling clojure.tools.nrepl.transport
Compiling mranderson045.cljfmt.v0v3v0.rewrite-clj.v0v4v12.rewrite-clj.node.token
Compiling clojure.test.tap
Compiling mranderson045.cljfmt.v0v3v0.rewrite-clj.v0v4v12.rewrite-clj.zip.walk
Compiling clojure.repl
Compiling cider.nrepl.middleware.util.inspect
Compiling mranderson045.cljfmt.v0v3v0.rewrite-clj.v0v4v12.rewrite-clj.node.string
Compiling clojure.tools.nrepl.middleware.interruptible-eval
Compiling mranderson045.cljs-tooling.v0v1v7.cljs-tooling.util.analysis
Compiling neko.-utils
Compiling neko.doc
Compiling cider.nrepl.middleware.pprint
Compiling cider.nrepl.middleware.apropos
Compilation succeeded.
Creating DEX....
Crunching resources...
Packaging resources...
Creating APK...
Signing APK with /Users/lucas-cleto/.android/debug.keystore ...
Aligning APK...
Installing APK...
Launching APK...
Binding device port 9999 to local port 9999 ...
```

```
$ /Users/lucas-cleto/Desktop/android-sdk-macosx/platform-tools/adb logcat
08-25 10:01:29.690  2147  2147 D AndroidRuntime: >>>>>> START com.android.internal.os.RuntimeInit uid 0 <<<<<<
08-25 10:01:29.690  2147  2147 D AndroidRuntime: CheckJNI is ON
08-25 10:01:29.710  2147  2147 I art     : JIT created with code_cache_capacity=2MB compile_threshold=1000
08-25 10:01:29.710  2147  2147 D ICU     : No timezone override file found: /data/misc/zoneinfo/current/icu/icu_tzdata.dat
08-25 10:01:29.730  2147  2147 E memtrack: Couldn't load memtrack module (No such file or directory)
08-25 10:01:29.730  2147  2147 E android.os.Debug: failed to load memtrack module: -2
08-25 10:01:29.730  2147  2147 I Radio-JNI: register_android_hardware_Radio DONE
08-25 10:01:29.740  2147  2147 D AndroidRuntime: Calling main entry com.android.commands.pm.Pm
08-25 10:01:29.750  2045  2057 D DefContainer: Copying /data/local/tmp/testapp.apk to base.apk
08-25 10:01:29.870  1338  1362 I PackageManager.DexOptimizer: Running dexopt (dex2oat) on: /data/app/vmdl2066180286.tmp/base.apk pkg=com.test.testapp.debug isa=x86_64 vmSafeMode=false debuggable=true oatDir = /data/app/vmdl2066180286.tmp/oat
08-25 10:01:29.880  2159  2159 W dex2oat : Unexpected CPU variant for X86 using defaults: x86_64
08-25 10:01:29.880  2159  2159 I dex2oat : /system/bin/dex2oat --debuggable
08-25 10:01:29.880  2159  2159 E cutils-trace: Error opening trace file: Permission denied (13)
08-25 10:01:31.460  2159  2159 I dex2oat : Method exceeds compiler instruction limit: 60156 in void clojure.core__init.load()
08-25 10:01:31.460  2159  2159 I dex2oat : Method exceeds compiler instruction limit: 60156 in void clojure.core__init.load()
08-25 10:01:33.000  2159  2159 W dex2oat : Compilation of java.lang.Object clojure.set$select$fn__7162.invoke(java.lang.Object, java.lang.Object) took 370ms
08-25 10:01:33.260  2159  2159 W dex2oat : Compilation of void clojure.tools.nrepl.middleware$describe_markdown$iter__2851__2855$fn__2856$fn__2857.<init>(java.lang.Object, java.lang.Object, int) took 210ms
08-25 10:01:34.030  2159  2159 W dex2oat : Compilation of clojure.lang.IMapEntry neko.data.MapLikeBundle.entryAt(java.lang.Object) took 380ms
08-25 10:01:38.810  2159  2159 I dex2oat : dex2oat took 8.930s (threads: 1) arena alloc=2MB java alloc=15MB native alloc=41MB free=3MB
08-25 10:01:38.880  1338  1352 I ActivityManager: Force stopping com.test.testapp.debug appid=10054 user=-1: uninstall pkg
08-25 10:01:38.880  1338  1352 I ActivityManager: Killing 2116:com.test.testapp.debug/u0a54 (adj 9): stop com.test.testapp.debug
08-25 10:01:38.920  1338  1350 W ActivityManager: Spurious death for ProcessRecord{18d887d 0:com.test.testapp.debug/u0a54}, curProc for 2116: null
08-25 10:01:38.920  1338  1752 W InputMethodManagerService: Got RemoteException sending setActive(false) notification to pid 2116 uid 10054
08-25 10:01:38.940  1338  1362 I PackageManager: Package com.test.testapp.debug codePath changed from /data/app/com.test.testapp.debug-1 to /data/app/com.test.testapp.debug-2; Retaining data and using new
08-25 10:01:38.940  1338  1352 I ActivityManager: Force stopping com.test.testapp.debug appid=10054 user=-1: replace pkg
08-25 10:01:38.940  1338  1362 W PackageManager: Code path for com.test.testapp.debug changing from /data/app/com.test.testapp.debug-1 to /data/app/com.test.testapp.debug-2
08-25 10:01:38.940  1338  1362 W PackageManager: Resource path for com.test.testapp.debug changing from /data/app/com.test.testapp.debug-1 to /data/app/com.test.testapp.debug-2
08-25 10:01:39.610  1338  1362 W Settings: Setting install_non_market_apps has moved from android.provider.Settings.Global to android.provider.Settings.Secure, returning read-only value.
08-25 10:01:39.610  1338  1362 I art     : Starting a blocking GC Explicit
08-25 10:01:39.610  1338  1362 I art     : Explicit concurrent mark sweep GC freed 28023(1883KB) AllocSpace objects, 9(180KB) LOS objects, 33% free, 6MB/10MB, paused 0 total 0
08-25 10:01:39.620  1338  1362 W PackageManager: Couldn't remove dex file for package:  at location /data/app/com.test.testapp.debug-1/base.apk, retcode=-1
08-25 10:01:39.620  1338  1362 I ActivityManager: Force stopping com.test.testapp.debug appid=10054 user=0: pkg removed
08-25 10:01:39.640  2147  2147 I art     : System.exit called, status: 0
08-25 10:01:39.640  2147  2147 I AndroidRuntime: VM exiting with result code 0.
08-25 10:01:39.960  1338  1357 I Choreographer: Skipped 31 frames!  The application may be doing too much work on its main thread.
08-25 10:01:39.960  1338  1362 W art     : Long monitor contention event with owner method=void com.android.server.wm.WindowAnimator$1.doFrame(long) from WindowAnimator.java:121 waiters=0 for 340ms
08-25 10:01:40.480  1338  1362 W art     : Long monitor contention event with owner method=void com.android.server.wm.WindowAnimator$1.doFrame(long) from WindowAnimator.java:121 waiters=0 for 520ms
08-25 10:01:40.480  1338  1357 W AppOps  : Finishing op nesting under-run: uid 1000 pkg android code 24 time=0 duration=0 nesting=0
08-25 10:01:40.490  1338  1338 D JobSchedulerService: Receieved: android.intent.action.PACKAGE_REMOVED
08-25 10:01:40.500  1338  1369 I InputReader: Reconfiguring input devices.  changes=0x00000010
08-25 10:01:40.510  1897  1897 W ContextImpl: Calling a method in the system process without a qualified user: android.app.ContextImpl.startService:1221 android.content.ContextWrapper.startService:581 android.content.ContextWrapper.startService:581 com.android.keychain.KeyChainBroadcastReceiver.onReceive:12 android.app.ActivityThread.handleReceiver:2725
08-25 10:01:40.510  1617  1617 D CarrierServiceBindHelper: Receive action: android.intent.action.PACKAGE_REMOVED
08-25 10:01:40.640  1338  1351 W VoiceInteractionManagerService: no available voice recognition services found for user 0
08-25 10:01:40.640  1617  1617 D CarrierServiceBindHelper: Receive action: android.intent.action.PACKAGE_ADDED
08-25 10:01:40.650  1617  1617 D CarrierServiceBindHelper: Receive action: android.intent.action.PACKAGE_REPLACED
08-25 10:01:40.650  1617  1617 D CarrierServiceBindHelper: mHandler: 3
08-25 10:01:40.650  1617  1617 D CarrierServiceBindHelper: mHandler: 3
08-25 10:01:40.650  1617  1617 D CarrierServiceBindHelper: mHandler: 3
08-25 10:01:40.650  1617  1617 D CarrierConfigLoader: mHandler: 9 phoneId: 0
08-25 10:01:40.990  2165  2165 D AndroidRuntime: >>>>>> START com.android.internal.os.RuntimeInit uid 0 <<<<<<
08-25 10:01:41.090  2165  2165 D AndroidRuntime: CheckJNI is ON
08-25 10:01:41.160  2165  2165 I art     : JIT created with code_cache_capacity=2MB compile_threshold=1000
08-25 10:01:41.170  2165  2165 D ICU     : No timezone override file found: /data/misc/zoneinfo/current/icu/icu_tzdata.dat
08-25 10:01:41.190  2165  2165 E memtrack: Couldn't load memtrack module (No such file or directory)
08-25 10:01:41.190  2165  2165 E android.os.Debug: failed to load memtrack module: -2
08-25 10:01:41.190  2165  2165 I Radio-JNI: register_android_hardware_Radio DONE
08-25 10:01:41.230  2165  2165 D AndroidRuntime: Calling main entry com.android.commands.am.Am
08-25 10:01:41.230  1338  1848 I ActivityManager: START u0 {flg=0x10000000 cmp=com.test.testapp.debug/com.test.testapp.SplashActivity} from uid 0 on display 0
08-25 10:01:41.370  2165  2165 D AndroidRuntime: Shutting down VM
08-25 10:01:41.390  2177  2177 I art     : Not late-enabling -Xcheck:jni (already on)
08-25 10:01:41.390  2177  2177 I art     : Late-enabling JIT
08-25 10:01:41.390  2177  2177 I art     : JIT created with code_cache_capacity=2MB compile_threshold=1000
08-25 10:01:41.400  1338  1513 I ActivityManager: Start proc 2177:com.test.testapp.debug/u0a54 for activity com.test.testapp.debug/com.test.testapp.SplashActivity
08-25 10:01:41.410  2177  2177 W System  : ClassLoader referenced unknown path: /data/app/com.test.testapp.debug-2/lib/x86_64
08-25 10:01:42.050  2177  2177 D gralloc_goldfish: Emulator without GPU emulation detected.
08-25 10:01:42.440  1338  1349 W art     : Long monitor contention event with owner method=void com.android.server.wm.WindowAnimator$1.doFrame(long) from WindowAnimator.java:121 waiters=0 for 320ms
08-25 10:01:43.310  1338  1349 W art     : Long monitor contention event with owner method=void com.android.server.wm.WindowAnimator$1.doFrame(long) from WindowAnimator.java:121 waiters=0 for 440ms
08-25 10:01:44.080  1338  1349 W art     : Long monitor contention event with owner method=void com.android.server.wm.WindowAnimator$1.doFrame(long) from WindowAnimator.java:121 waiters=0 for 380ms
08-25 10:01:44.440  1338  1349 W art     : Long monitor contention event with owner method=void com.android.server.wm.WindowAnimator$1.doFrame(long) from WindowAnimator.java:121 waiters=0 for 360ms
08-25 10:01:44.820  1338  1349 W art     : Long monitor contention event with owner method=void com.android.server.wm.WindowAnimator$1.doFrame(long) from WindowAnimator.java:121 waiters=0 for 380ms
08-25 10:01:45.210  1338  1349 W art     : Long monitor contention event with owner method=void com.android.server.wm.WindowAnimator$1.doFrame(long) from WindowAnimator.java:121 waiters=0 for 390ms
08-25 10:01:45.590  1338  1349 W art     : Long monitor contention event with owner method=void com.android.server.wm.WindowAnimator$1.doFrame(long) from WindowAnimator.java:121 waiters=0 for 380ms
08-25 10:01:45.970  1338  1349 W art     : Long monitor contention event with owner method=void com.android.server.wm.WindowAnimator$1.doFrame(long) from WindowAnimator.java:121 waiters=0 for 380ms
08-25 10:01:46.270  2177  2191 D DalvikClojureCompiler: CACHED DIRECTORY: /data/user/0/com.test.testapp.debug/cache/clojure_repl
08-25 10:01:46.340  2192  2192 W dex2oat : Unexpected CPU variant for X86 using defaults: x86_64
08-25 10:01:46.340  2192  2192 I dex2oat : /system/bin/dex2oat --debuggable --compiler-filter=interpret-only --dex-file=/data/user/0/com.test.testapp.debug/cache/clojure_repl/repl--442625193.dex --oat-file=/data/user/0/com.test.testapp.debug/cache/clojure_repl/repl-opt--442625193.dex
08-25 10:01:46.340  2192  2192 E cutils-trace: Error opening trace file: Permission denied (13)
08-25 10:01:46.420  2192  2192 I dex2oat : dex2oat took 80ms (threads: 1) arena alloc=0B java alloc=21KB native alloc=501KB free=522KB
08-25 10:01:46.570  2194  2194 W dex2oat : Unexpected CPU variant for X86 using defaults: x86_64
08-25 10:01:46.570  2194  2194 I dex2oat : /system/bin/dex2oat --debuggable --compiler-filter=interpret-only --dex-file=/data/user/0/com.test.testapp.debug/cache/clojure_repl/repl-1916668207.dex --oat-file=/data/user/0/com.test.testapp.debug/cache/clojure_repl/repl-opt-1916668207.dex
08-25 10:01:46.570  2194  2194 E cutils-trace: Error opening trace file: Permission denied (13)
08-25 10:01:46.580  2194  2194 I dex2oat : dex2oat took 10ms (threads: 1) arena alloc=0B java alloc=25KB native alloc=501KB free=522KB
08-25 10:01:46.780  1338  1349 W art     : Long monitor contention event with owner method=void com.android.server.wm.WindowAnimator$1.doFrame(long) from WindowAnimator.java:121 waiters=0 for 420ms
08-25 10:01:47.250  2177  2188 I art     : Background sticky concurrent mark sweep GC freed 96819(3MB) AllocSpace objects, 0(0B) LOS objects, 24% free, 11MB/14MB, paused 0 total 110ms
08-25 10:01:47.560  1338  1848 W art     : Long monitor contention event with owner method=void com.android.server.wm.WindowAnimator$1.doFrame(long) from WindowAnimator.java:121 waiters=1 for 400ms
08-25 10:01:47.570  1338  1357 I ActivityManager: Displayed com.test.testapp.debug/com.test.testapp.SplashActivity: +6s190ms
08-25 10:01:47.570  2177  2177 I Choreographer: Skipped 326 frames!  The application may be doing too much work on its main thread.
08-25 10:01:50.290  2177  2188 I art     : Background partial concurrent mark sweep GC freed 76237(3MB) AllocSpace objects, 0(0B) LOS objects, 22% free, 13MB/17MB, paused 0 total 150ms
08-25 10:01:51.380  1338  1352 W ActivityManager: Launch timeout has expired, giving up wake lock!
08-25 10:01:54.260  2177  2188 I art     : Background sticky concurrent mark sweep GC freed 66990(2MB) AllocSpace objects, 0(0B) LOS objects, 12% free, 16MB/19MB, paused 0 total 110ms
08-25 10:01:54.400  2177  2191 E AndroidRuntime: FATAL EXCEPTION: ClojureLoadingThread
08-25 10:01:54.400  2177  2191 E AndroidRuntime: Process: com.test.testapp.debug, PID: 2177
08-25 10:01:54.400  2177  2191 E AndroidRuntime: java.lang.ExceptionInInitializerError
08-25 10:01:54.400  2177  2191 E AndroidRuntime: 	at java.lang.Class.classForName(Native Method)
08-25 10:01:54.400  2177  2191 E AndroidRuntime: 	at java.lang.Class.forName(Class.java:324)
08-25 10:01:54.400  2177  2191 E AndroidRuntime: 	at clojure.lang.RT.classForName(RT.java:2201)
08-25 10:01:54.400  2177  2191 E AndroidRuntime: 	at clojure.lang.RT.classForName(RT.java:2210)
08-25 10:01:54.400  2177  2191 E AndroidRuntime: 	at clojure.lang.RT.loadClassForName(RT.java:2229)
08-25 10:01:54.400  2177  2191 E AndroidRuntime: 	at clojure.lang.RT.load(RT.java:461)
08-25 10:01:54.400  2177  2191 E AndroidRuntime: 	at clojure.lang.RT.load(RT.java:437)
08-25 10:01:54.400  2177  2191 E AndroidRuntime: 	at clojure.core$load$fn__5442.invoke(core.clj:5858)
08-25 10:01:54.400  2177  2191 E AndroidRuntime: 	at clojure.core$load.doInvoke(core.clj:5857)
08-25 10:01:54.400  2177  2191 E AndroidRuntime: 	at clojure.lang.RestFn.invoke(RestFn.java:408)
08-25 10:01:54.400  2177  2191 E AndroidRuntime: 	at clojure.core$load_one.invoke(core.clj:5663)
08-25 10:01:54.400  2177  2191 E AndroidRuntime: 	at clojure.core$load_lib$fn__5391.invoke(core.clj:5703)
08-25 10:01:54.400  2177  2191 E AndroidRuntime: 	at clojure.core$load_lib.doInvoke(core.clj:5702)
08-25 10:01:54.400  2177  2191 E AndroidRuntime: 	at clojure.lang.RestFn.applyTo(RestFn.java:142)
08-25 10:01:54.400  2177  2191 E AndroidRuntime: 	at clojure.core$apply.invoke(core.clj:630)
08-25 10:01:54.400  2177  2191 E AndroidRuntime: 	at clojure.core$load_libs.doInvoke(core.clj:5741)
08-25 10:01:54.400  2177  2191 E AndroidRuntime: 	at clojure.lang.RestFn.applyTo(RestFn.java:137)
08-25 10:01:54.400  2177  2191 E AndroidRuntime: 	at clojure.core$apply.invoke(core.clj:630)
08-25 10:01:54.400  2177  2191 E AndroidRuntime: 	at clojure.core$require.doInvoke(core.clj:5824)
08-25 10:01:54.400  2177  2191 E AndroidRuntime: 	at clojure.lang.RestFn.invoke(RestFn.java:703)
08-25 10:01:54.400  2177  2191 E AndroidRuntime: 	at cider.nrepl.middleware.format$loading__5334__auto____6890.invoke(format.clj:1)
08-25 10:01:54.400  2177  2191 E AndroidRuntime: 	at cider.nrepl.middleware.format__init.load(Unknown Source)
08-25 10:01:54.400  2177  2191 E AndroidRuntime: 	at cider.nrepl.middleware.format__init.<clinit>(Unknown Source)
08-25 10:01:54.400  2177  2191 E AndroidRuntime: 	at java.lang.Class.classForName(Native Method)
08-25 10:01:54.400  2177  2191 E AndroidRuntime: 	at java.lang.Class.forName(Class.java:324)
08-25 10:01:54.400  2177  2191 E AndroidRuntime: 	at clojure.lang.RT.classForName(RT.java:2201)
08-25 10:01:54.400  2177  2191 E AndroidRuntime: 	at clojure.lang.RT.classForName(RT.java:2210)
08-25 10:01:54.400  2177  2191 E AndroidRuntime: 	at clojure.lang.RT.loadClassForName(RT.java:2229)
08-25 10:01:54.400  2177  2191 E AndroidRuntime: 	at clojure.lang.RT.load(RT.java:461)
08-25 10:01:54.400  2177  2191 E AndroidRuntime: 	at clojure.lang.RT.load(RT.java:437)
08-25 10:01:54.400  2177  2191 E AndroidRuntime: 	at clojure.core$load$fn__5442.invoke(core.clj:5858)
08-25 10:01:54.400  2177  2191 E AndroidRuntime: 	at clojure.core$load.doInvoke(core.clj:5857)
08-25 10:01:54.400  2177  2191 E AndroidRuntime: 	at clojure.lang.RestFn.invoke(RestFn.java:408)
08-25 10:01:54.400  2177  2191 E AndroidRuntime: 	at clojure.core$load_one.invoke(core.clj:5663)
08-25 10:01:54.400  2177  2191 E AndroidRuntime: 	at clojure.core$load_lib$fn__5391.invoke(core.clj:5703)
08-25 10:01:54.400  2177  2191 E AndroidRuntime: 	at clojure.core$load_lib.doInvoke(core.clj:5702)
08-25 10:01:54.400  2177  2191 E AndroidRuntime: 	at clojure.lang.RestFn.applyTo(RestFn.java:142)
08-25 10:01:54.400  2177  2191 E AndroidRuntime: 	at clojure.core$apply.invoke(core.clj:630)
08-25 10:01:54.400  2177  2191 E AndroidRuntime: 	at clojure.core$load_libs.doInvoke(core.clj:5741)
08-25 10:01:54.400  2177  2191 E AndroidRuntime: 	at clojure.lang.RestFn.applyTo(RestFn.java:137)
08-25 10:01:54.400  2177  2191 E AndroidRuntime: 	at clojure.core$apply.invoke(core.clj:630)
08-25 10:01:54.400  2177  2191 E AndroidRuntime: 	at clojure.core$require.doInvoke(core.clj:5824)
08-25 10:01:54.400  2177  2191 E AndroidRuntime: 	at clojure.lang.RestFn.invoke(RestFn.java:408)
08-25 10:01:54.400  2177  2191 E AndroidRuntime: 	at neko.tools.repl$start_repl$fn__6482$fn__6483.invoke(repl.clj:77)
08-25 10:01:54.400  2177  2191 E AndroidRuntime: 	at clojure.core$map$fn__4547.invoke(core.clj:2616)
08-25 10:01:54.400  2177  2191 E AndroidRuntime: 	at clojure.lang.LazySeq.sval(LazySeq.java:40)
08-25 10:01:54.400  2177  2191 E AndroidRuntime: 	at clojure.lang.LazySeq.seq(LazySeq.java:49)
08-25 10:01:54.400  2177  2191 E AndroidRuntime: 	at clojure.lang.RT.seq(RT.java:534)
08-25 10:01:54.400  2177  2191 E AndroidRuntime: 	at clojure.core$seq__4122.invoke(core.clj:135)
08-25 10:01:54.400  2177  2191 E AndroidRuntime: 	at clojure.core$apply.invoke(core.clj:628)
08-25 10:01:54.400  2177  2191 E AndroidRuntime: 	at neko.tools.repl$start_repl$fn__6482.invoke(repl.clj:75)
08-25 10:01:54.400  2177  2191 E AndroidRuntime: 	at clojure.core$with_redefs_fn.invoke(core.clj:7185)
08-25 10:01:54.400  2177  2191 E AndroidRuntime: 	at neko.tools.repl$start_repl.doInvoke(repl.clj:72)
08-25 10:01:54.400  2177  2191 E AndroidRuntime: 	at clojure.lang.RestFn.applyTo(RestFn.java:139)
08-25 10:01:54.400  2177  2191 E AndroidRuntime: 	at clojure.core$apply.invoke(core.clj:630)
08-25 10:01:54.400  2177  2191 E AndroidRuntime: 	at neko.tools.repl$init.doInvoke(repl.clj:102)
08-25 10:01:54.400  2177  2191 E AndroidRuntime: 	at clojure.lang.RestFn.invoke(RestFn.java:397)
08-25 10:01:54.400  2177  2191 E AndroidRuntime: 	at clojure.lang.Var.invoke(Var.java:375)
08-25 10:01:54.400  2177  2191 E AndroidRuntime: 	at neko.App.loadClojure(App.java:40)
08-25 10:01:54.400  2177  2191 E AndroidRuntime: 	at neko.App$1.run(App.java:51)
08-25 10:01:54.400  2177  2191 E AndroidRuntime: 	at java.lang.Thread.run(Thread.java:818)
08-25 10:01:54.400  2177  2191 E AndroidRuntime: Caused by: java.lang.IllegalArgumentException: No implementation of method: :make-reader of protocol: #'clojure.java.io/IOFactory found for class: nil
08-25 10:01:54.400  2177  2191 E AndroidRuntime: 	at clojure.core$_cache_protocol_fn.invoke(core_deftype.clj:554)
08-25 10:01:54.400  2177  2191 E AndroidRuntime: 	at clojure.java.io$fn__8970$G__8946__8977.invoke(io.clj:69)
08-25 10:01:54.400  2177  2191 E AndroidRuntime: 	at clojure.java.io$reader.doInvoke(io.clj:102)
08-25 10:01:54.400  2177  2191 E AndroidRuntime: 	at clojure.lang.RestFn.invoke(RestFn.java:410)
08-25 10:01:54.400  2177  2191 E AndroidRuntime: 	at clojure.lang.AFn.applyToHelper(AFn.java:154)
08-25 10:01:54.400  2177  2191 E AndroidRuntime: 	at clojure.lang.RestFn.applyTo(RestFn.java:132)
08-25 10:01:54.400  2177  2191 E AndroidRuntime: 	at clojure.core$apply.invoke(core.clj:630)
08-25 10:01:54.400  2177  2191 E AndroidRuntime: 	at clojure.core$slurp.doInvoke(core.clj:6645)
08-25 10:01:54.400  2177  2191 E AndroidRuntime: 	at clojure.lang.RestFn.invoke(RestFn.java:410)
08-25 10:01:54.400  2177  2191 E AndroidRuntime: 	at clojure.core$comp$fn__4489.invoke(core.clj:2432)
08-25 10:01:54.400  2177  2191 E AndroidRuntime: 	at clojure.core$comp$fn__4489.invoke(core.clj:2432)
08-25 10:01:54.400  2177  2191 E AndroidRuntime: 	at mranderson045.cljfmt.v0v3v0.cljfmt.core__init.load(Unknown Source)
08-25 10:01:54.400  2177  2191 E AndroidRuntime: 	at mranderson045.cljfmt.v0v3v0.cljfmt.core__init.<clinit>(Unknown Source)
08-25 10:01:54.400  2177  2191 E AndroidRuntime: 	... 61 more
08-25 10:01:54.400  1338  1752 W ActivityManager:   Force finishing activity com.test.testapp.debug/com.test.testapp.SplashActivity
08-25 10:01:54.510   995   995 D gralloc : Registering a buffer in the process that created it. This may cause memory ordering problems.
08-25 10:01:54.510   995   995 E libEGL  : called unimplemented OpenGL ES API
08-25 10:01:54.510   995   995 E SurfaceFlinger: glCheckFramebufferStatusOES error 1605930612
08-25 10:01:54.510   995   995 E SurfaceFlinger: got GL_FRAMEBUFFER_COMPLETE_OES error while taking screenshot
08-25 10:01:54.600  1338  1348 I art     : Background partial concurrent mark sweep GC freed 949(51KB) AllocSpace objects, 0(0B) LOS objects, 33% free, 6MB/10MB, paused 40ms total 40ms
08-25 10:01:54.860  1338  1354 W art     : Long monitor contention event with owner method=int com.android.server.wm.WindowManagerService.relayoutWindow(com.android.server.wm.Session, android.view.IWindow, int, android.view.WindowManager$LayoutParams, int, int, int, int, android.graphics.Rect, android.graphics.Rect, android.graphics.Rect, android.graphics.Rect, android.graphics.Rect, android.graphics.Rect, android.content.res.Configuration, android.view.Surface) from WindowManagerService.java:3097 waiters=0 for 110ms
08-25 10:01:55.260  1338  1353 W art     : Long monitor contention event with owner method=void com.android.server.wm.WindowAnimator$1.doFrame(long) from WindowAnimator.java:121 waiters=0 for 320ms
08-25 10:01:56.390  1338  1777 W art     : Long monitor contention event with owner method=void com.android.server.wm.WindowAnimator$1.doFrame(long) from WindowAnimator.java:121 waiters=1 for 730ms
08-25 10:01:56.720  1338  1513 W art     : Long monitor contention event with owner method=void com.android.server.wm.WindowAnimator$1.doFrame(long) from WindowAnimator.java:121 waiters=0 for 270ms
08-25 10:02:04.200  2177  2191 I Process : Sending signal. PID: 2177 SIG: 9
08-25 10:02:04.210  1338  1350 E JavaBinder: !!! FAILED BINDER TRANSACTION !!!  (parcel size = 104)
08-25 10:02:04.210  1338  1350 W InputMethodManagerService: Got RemoteException sending setActive(false) notification to pid 2177 uid 10054
08-25 10:02:04.210  1338  1350 E JavaBinder: !!! FAILED BINDER TRANSACTION !!!  (parcel size = 104)
08-25 10:02:04.210  1338  1385 W AudioTrack: AUDIO_OUTPUT_FLAG_FAST denied by client; transfer 4, track 48000 Hz, output 44100 Hz
08-25 10:02:04.240  1338  1883 I ActivityManager: Process com.test.testapp.debug (pid 2177) has died
08-25 10:02:05.500  1338  1357 W AppOps  : Finishing op nesting under-run: uid 1000 pkg android code 24 time=0 duration=0 nesting=0
```
