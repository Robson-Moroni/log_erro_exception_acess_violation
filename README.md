#
# A fatal error has been detected by the Java Runtime Environment:
#
#  EXCEPTION_ACCESS_VIOLATION (0xc0000005) at pc=0x000000007110b5db, pid=8692, tid=0x0000000000001ea0
#
# JRE version: Java(TM) SE Runtime Environment (8.0_291-b10) (build 1.8.0_291-b10)
# Java VM: Java HotSpot(TM) 64-Bit Server VM (25.291-b10 mixed mode windows-amd64 compressed oops)
# Problematic frame:
# C  [jSSC-2.8_x86_64.dll+0xb5db]
#
# Failed to write core dump. Minidumps are not enabled by default on client versions of Windows
#
# If you would like to submit a bug report, please visit:
#   http://bugreport.java.com/bugreport/crash.jsp
# The crash happened outside the Java Virtual Machine in native code.
# See problematic frame for where to report the bug.
#

---------------  T H R E A D  ---------------

Current thread (0x0000023dc8e85800):  JavaThread "main" [_thread_in_native, id=7840, stack(0x00000071d7c00000,0x00000071d7d00000)]

siginfo: ExceptionCode=0xc0000005, reading address 0xffffffffe883a3bd

Registers:
RAX=0xffffffffe883a3bd, RBX=0x00000071d7cfdb20, RCX=0x0000023df67c38bc, RDX=0x000000007110c52c
RSP=0x00000071d7cfdab0, RBP=0x00000071d7cfdc30, RSI=0x0000023dc8e85a00, RDI=0x0000000000000d98
R8 =0x0000000000000000, R9 =0x0000000000000000, R10=0x0000000000000004, R11=0x0000000000000080
R12=0x00000071d7cfdce0, R13=0x0000023de623e600, R14=0x00000071d7cfdbe0, R15=0x0000023dc8e85800
RIP=0x000000007110b5db, EFLAGS=0x0000000000000242

Top of Stack: (sp=0x00000071d7cfdab0)
0x00000071d7cfdab0:   00000071d7cfdce0 0000023de623e600
0x00000071d7cfdac0:   000000007110b230 0000023de623e600
0x00000071d7cfdad0:   00000071d7cfdaf0 0000000000000004
0x00000071d7cfdae0:   0000023dc8e85a00 0000000000000d98
0x00000071d7cfdaf0:   00000071d7cfdc30 0000000071112590
0x00000071d7cfdb00:   0000000000000000 0000000000000000
0x00000071d7cfdb10:   0000000000000000 0000000000000000
0x00000071d7cfdb20:   0000000000000000 0000000000000000
0x00000071d7cfdb30:   0000000000000000 0000000000000000
0x00000071d7cfdb40:   0000000000000000 0000000000000000
0x00000071d7cfdb50:   0000000071113500 0000000071113be8
0x00000071d7cfdb60:   00000071d7cfdb90 0000000071112641
0x00000071d7cfdb70:   00000071d7cfdb00 0000000000000000
0x00000071d7cfdb80:   0000000000000000 0000000000000000
0x00000071d7cfdb90:   00000071d7cfdc30 0000000071101595
0x00000071d7cfdba0:   000000000000001c 0000000071101521 

Instructions: (pc=0x000000007110b5db)
0x000000007110b5bb:   c5 0f 1f 40 00 55 57 56 53 48 83 ec 28 48 8b 05
0x000000007110b5cb:   39 33 01 00 48 89 cb 48 85 c0 0f 84 c5 00 00 00
0x000000007110b5db:   8b 38 85 ff 0f 88 ab 00 00 00 48 8b 05 1c 33 01
0x000000007110b5eb:   00 48 85 c0 0f 84 bc 00 00 00 8b 30 85 f6 74 57 


Register to memory mapping:

RAX=0xffffffffe883a3bd is an unknown value
RBX=0x00000071d7cfdb20 is pointing into the stack for thread: 0x0000023dc8e85800
RCX=0x0000023df67c38bc is an unknown value
RDX=0x000000007110c52c is an unknown value
RSP=0x00000071d7cfdab0 is pointing into the stack for thread: 0x0000023dc8e85800
RBP=0x00000071d7cfdc30 is pointing into the stack for thread: 0x0000023dc8e85800
RSI=0x0000023dc8e85a00 is an unknown value
RDI=0x0000000000000d98 is an unknown value
R8 =0x0000000000000000 is an unknown value
R9 =0x0000000000000000 is an unknown value
R10=0x0000000000000004 is an unknown value
R11=0x0000000000000080 is an unknown value
R12=0x00000071d7cfdce0 is pointing into the stack for thread: 0x0000023dc8e85800
R13=0x0000023de623e600 is an unknown value
R14=0x00000071d7cfdbe0 is pointing into the stack for thread: 0x0000023dc8e85800
R15=0x0000023dc8e85800 is a thread


Stack: [0x00000071d7c00000,0x00000071d7d00000],  sp=0x00000071d7cfdab0,  free space=1014k
Native frames: (J=compiled Java code, j=interpreted, Vv=VM code, C=native code)
C  [jSSC-2.8_x86_64.dll+0xb5db]
C  [jSSC-2.8_x86_64.dll+0x12590]
C  [jSSC-2.8_x86_64.dll+0x1595]
C  0x0000023dd01d990e

Java frames: (J=compiled Java code, j=interpreted, Vv=VM code)
j  jssc.SerialNativeInterface.openPort(Ljava/lang/String;Z)J+0
j  jssc.SerialPort.openPort()Z+65
j  br.com.germantech.ecf.aplicacao.services.BalancaService.testarBalanca()Ljava/math/BigDecimal;+36
j  br.com.germantech.ecf.telas.editors.BalancaEditor$11.widgetSelected(Lorg/eclipse/swt/events/SelectionEvent;)V+19
J 13289 C1 org.eclipse.swt.widgets.TypedListener.handleEvent(Lorg/eclipse/swt/widgets/Event;)V (1291 bytes) @ 0x0000023dd27d82ac [0x0000023dd27d3de0+0x44cc]
J 13954 C2 org.eclipse.swt.widgets.EventTable.sendEvent(Lorg/eclipse/swt/widgets/Event;)V (592 bytes) @ 0x0000023dd293110c [0x0000023dd2931060+0xac]
J 11640 C1 org.eclipse.swt.widgets.Display.sendEvent(Lorg/eclipse/swt/widgets/EventTable;Lorg/eclipse/swt/widgets/Event;)V (34 bytes) @ 0x0000023dd234320c [0x0000023dd2343120+0xec]
J 13068 C1 org.eclipse.swt.widgets.Display.runDeferredEvents()Z (109 bytes) @ 0x0000023dd26e31c4 [0x0000023dd26e29c0+0x804]
J 14190 C1 org.eclipse.swt.widgets.Display.readAndDispatch()Z (94 bytes) @ 0x0000023dd11e8da4 [0x0000023dd11e8700+0x6a4]
j  org.eclipse.e4.ui.internal.workbench.swt.PartRenderingEngine$5.run()V+564
j  org.eclipse.core.databinding.observable.Realm.runWithDefault(Lorg/eclipse/core/databinding/observable/Realm;Ljava/lang/Runnable;)V+12
j  org.eclipse.e4.ui.internal.workbench.swt.PartRenderingEngine.run(Lorg/eclipse/e4/ui/model/application/MApplicationElement;Lorg/eclipse/e4/core/contexts/IEclipseContext;)Ljava/lang/Object;+57
j  org.eclipse.e4.ui.internal.workbench.E4Workbench.createAndRunUI(Lorg/eclipse/e4/ui/model/application/MApplicationElement;)V+20
j  org.eclipse.ui.internal.Workbench.lambda$3(Lorg/eclipse/swt/widgets/Display;Lorg/eclipse/ui/application/WorkbenchAdvisor;[I)V+341
j  org.eclipse.ui.internal.Workbench$$Lambda$45.run()V+12
j  org.eclipse.core.databinding.observable.Realm.runWithDefault(Lorg/eclipse/core/databinding/observable/Realm;Ljava/lang/Runnable;)V+12
j  org.eclipse.ui.internal.Workbench.createAndRunWorkbench(Lorg/eclipse/swt/widgets/Display;Lorg/eclipse/ui/application/WorkbenchAdvisor;)I+16
j  org.eclipse.ui.PlatformUI.createAndRunWorkbench(Lorg/eclipse/swt/widgets/Display;Lorg/eclipse/ui/application/WorkbenchAdvisor;)I+2
j  br.com.germantech.ecf.aplicacao.internal.Application.start(Lorg/eclipse/equinox/app/IApplicationContext;)Ljava/lang/Object;+54
j  org.eclipse.equinox.internal.app.EclipseAppHandle.run(Ljava/lang/Object;)Ljava/lang/Object;+135
j  org.eclipse.equinox.internal.app.MainApplicationLauncher.run(Ljava/lang/Object;)Ljava/lang/Object;+19
j  org.eclipse.core.runtime.internal.adaptor.EclipseAppLauncher.runApplication(Ljava/lang/Object;)Ljava/lang/Object;+85
j  org.eclipse.core.runtime.internal.adaptor.EclipseAppLauncher.start(Ljava/lang/Object;)Ljava/lang/Object;+82
j  org.eclipse.core.runtime.adaptor.EclipseStarter.run(Ljava/lang/Object;)Ljava/lang/Object;+105
j  org.eclipse.core.runtime.adaptor.EclipseStarter.run([Ljava/lang/String;Ljava/lang/Runnable;)Ljava/lang/Object;+132
v  ~StubRoutines::call_stub
j  sun.reflect.NativeMethodAccessorImpl.invoke0(Ljava/lang/reflect/Method;Ljava/lang/Object;[Ljava/lang/Object;)Ljava/lang/Object;+0
j  sun.reflect.NativeMethodAccessorImpl.invoke(Ljava/lang/Object;[Ljava/lang/Object;)Ljava/lang/Object;+100
j  sun.reflect.DelegatingMethodAccessorImpl.invoke(Ljava/lang/Object;[Ljava/lang/Object;)Ljava/lang/Object;+6
j  java.lang.reflect.Method.invoke(Ljava/lang/Object;[Ljava/lang/Object;)Ljava/lang/Object;+56
j  org.eclipse.equinox.launcher.Main.invokeFramework([Ljava/lang/String;[Ljava/net/URL;)V+205
j  org.eclipse.equinox.launcher.Main.basicRun([Ljava/lang/String;)V+160
j  org.eclipse.equinox.launcher.Main.run([Ljava/lang/String;)I+4
j  org.eclipse.equinox.launcher.Main.main([Ljava/lang/String;)V+10
v  ~StubRoutines::call_stub

---------------  P R O C E S S  ---------------

Java Threads: ( => current thread )
  0x0000023deb3ca800 JavaThread "Worker-4" [_thread_blocked, id=9508, stack(0x00000071da000000,0x00000071da100000)]
  0x0000023deb3cb000 JavaThread "EventAdmin Async Event Dispatcher Thread" daemon [_thread_blocked, id=9988, stack(0x00000071d9900000,0x00000071d9a00000)]
  0x0000023deb3c7800 JavaThread "Worker-3" [_thread_blocked, id=3860, stack(0x00000071d7b00000,0x00000071d7c00000)]
  0x0000023deb3c8000 JavaThread "Worker-2" [_thread_blocked, id=8408, stack(0x00000071d7a00000,0x00000071d7b00000)]
  0x0000023deb3bf000 JavaThread "AWT-Windows" daemon [_thread_in_native, id=7240, stack(0x00000071d9f00000,0x00000071da000000)]
  0x0000023deb3c0000 JavaThread "Java2D Disposer" daemon [_thread_blocked, id=8380, stack(0x00000071d9400000,0x00000071d9500000)]
  0x0000023de4441800 JavaThread "Worker-1" [_thread_blocked, id=9076, stack(0x00000071d8e00000,0x00000071d8f00000)]
  0x0000023de443e800 JavaThread "EMF Reference Cleaner" daemon [_thread_blocked, id=2812, stack(0x00000071d8d00000,0x00000071d8e00000)]
  0x0000023de6714000 JavaThread "Gogo shell" [_thread_blocked, id=1956, stack(0x00000071d9800000,0x00000071d9900000)]
  0x0000023de5994800 JavaThread "Worker-0" [_thread_blocked, id=6464, stack(0x00000071d9700000,0x00000071d9800000)]
  0x0000023de5e7f000 JavaThread "Worker-JM" [_thread_blocked, id=9012, stack(0x00000071d9600000,0x00000071d9700000)]
  0x0000023de6f27000 JavaThread "SCR Component Actor" daemon [_thread_blocked, id=7568, stack(0x00000071d9500000,0x00000071d9600000)]
  0x0000023de6327800 JavaThread "Bundle File Closer" daemon [_thread_blocked, id=3568, stack(0x00000071d9300000,0x00000071d9400000)]
  0x0000023de59db800 JavaThread "Start Level: Equinox Container: 202594f7-b3d9-4f90-853e-a94eb4ad646e" daemon [_thread_blocked, id=9140, stack(0x00000071d9200000,0x00000071d9300000)]
  0x0000023de5976800 JavaThread "Refresh Thread: Equinox Container: 202594f7-b3d9-4f90-853e-a94eb4ad646e" daemon [_thread_blocked, id=9332, stack(0x00000071d9100000,0x00000071d9200000)]
  0x0000023de5917800 JavaThread "Framework Event Dispatcher: Equinox Container: 202594f7-b3d9-4f90-853e-a94eb4ad646e" daemon [_thread_blocked, id=9316, stack(0x00000071d9000000,0x00000071d9100000)]
  0x0000023de58be800 JavaThread "Active Thread: Equinox Container: 202594f7-b3d9-4f90-853e-a94eb4ad646e" [_thread_blocked, id=8828, stack(0x00000071d8f00000,0x00000071d9000000)]
  0x0000023de3c1d800 JavaThread "Service Thread" daemon [_thread_blocked, id=10192, stack(0x00000071d8b00000,0x00000071d8c00000)]
  0x0000023de3ba1000 JavaThread "C1 CompilerThread2" daemon [_thread_blocked, id=9256, stack(0x00000071d8a00000,0x00000071d8b00000)]
  0x0000023de3b9f800 JavaThread "C2 CompilerThread1" daemon [_thread_blocked, id=5868, stack(0x00000071d8900000,0x00000071d8a00000)]
  0x0000023de3b9f000 JavaThread "C2 CompilerThread0" daemon [_thread_blocked, id=9552, stack(0x00000071d8800000,0x00000071d8900000)]
  0x0000023de3b4f000 JavaThread "Attach Listener" daemon [_thread_blocked, id=2412, stack(0x00000071d8700000,0x00000071d8800000)]
  0x0000023de3b98800 JavaThread "Signal Dispatcher" daemon [_thread_blocked, id=1540, stack(0x00000071d8600000,0x00000071d8700000)]
  0x0000023de3b97800 JavaThread "Surrogate Locker Thread (Concurrent GC)" daemon [_thread_blocked, id=5336, stack(0x00000071d8500000,0x00000071d8600000)]
  0x0000023de3b29800 JavaThread "Finalizer" daemon [_thread_blocked, id=9968, stack(0x00000071d8400000,0x00000071d8500000)]
  0x0000023de3b21000 JavaThread "Reference Handler" daemon [_thread_blocked, id=8176, stack(0x00000071d8300000,0x00000071d8400000)]
=>0x0000023dc8e85800 JavaThread "main" [_thread_in_native, id=7840, stack(0x00000071d7c00000,0x00000071d7d00000)]

Other Threads:
  0x0000023de3b1b000 VMThread [stack: 0x00000071d8200000,0x00000071d8300000] [id=8412]
  0x0000023de3c39800 WatcherThread [stack: 0x00000071d8c00000,0x00000071d8d00000] [id=7716]

VM state:not at safepoint (normal execution)

VM Mutex/Monitor currently owned by a thread: None

heap address: 0x00000000c0000000, size: 1024 MB, Compressed Oops mode: 32-bit
Narrow klass base: 0x0000000000000000, Narrow klass shift: 3
Compressed class space size: 1073741824 Address: 0x0000000100000000

Heap:
 par new generation   total 125120K, used 39738K [0x00000000c0000000, 0x00000000c8000000, 0x00000000c8000000)
  eden space 119168K,  28% used [0x00000000c0000000, 0x00000000c20feb20, 0x00000000c7460000)
  from space 5952K, 100% used [0x00000000c7a30000, 0x00000000c8000000, 0x00000000c8000000)
  to   space 5952K,   0% used [0x00000000c7460000, 0x00000000c7460000, 0x00000000c7a30000)
 concurrent mark-sweep generation total 176128K, used 94671K [0x00000000c8000000, 0x00000000d2c00000, 0x0000000100000000)
 Metaspace       used 91288K, capacity 98233K, committed 98440K, reserved 1134592K
  class space    used 10999K, capacity 12844K, committed 12936K, reserved 1048576K

Card table byte_map: [0x0000023ddf680000,0x0000023ddf890000] byte_map_base: 0x0000023ddf080000

Marking Bits: (CMSBitMap*) 0x0000023dc8ee2648
 Bits: [0x0000023ddfea0000, 0x0000023de0ca0000)

Mod Union Table: (CMSBitMap*) 0x0000023dc8ee2708
 Bits: [0x0000023de0cb0000, 0x0000023de0ce8000)

Polling page: 0x0000023dd0140000

CodeCache: size=245760Kb used=38467Kb max_used=40429Kb free=207292Kb
 bounds [0x0000023dd01c0000, 0x0000023dd2980000, 0x0000023ddf1c0000]
 total_blobs=11876 nmethods=10950 adapters=835
 compilation: enabled

Compilation events (10 events):
Event: 103.077 Thread 0x0000023de3b9f000 nmethod 14217 0x0000023dd27f5a90 code [0x0000023dd27f5bc0, 0x0000023dd27f5c58]
Event: 103.086 Thread 0x0000023de3ba1000 nmethod 14216 0x0000023dd2825a90 code [0x0000023dd2826000, 0x0000023dd2829d90]
Event: 103.100 Thread 0x0000023de3ba1000 14218       3       org.eclipse.ui.internal.Workbench::getThemeManager (4 bytes)
Event: 103.102 Thread 0x0000023de3ba1000 nmethod 14218 0x0000023dd09b27d0 code [0x0000023dd09b2960, 0x0000023dd09b2dd0]
Event: 103.109 Thread 0x0000023de3ba1000 14220       3       org.eclipse.e4.ui.css.swt.properties.css2.CSSPropertyBackgroundSWTHandler::applyCSSPropertyBackgroundColor (257 bytes)
Event: 103.118 Thread 0x0000023de3ba1000 nmethod 14220 0x0000023dd1fc67d0 code [0x0000023dd1fc6d40, 0x0000023dd1fcaa90]
Event: 103.125 Thread 0x0000023de3ba1000 14221       3       org.eclipse.swt.widgets.Control::getEnabled (12 bytes)
Event: 103.125 Thread 0x0000023de3ba1000 nmethod 14221 0x0000023dd0723750 code [0x0000023dd07238c0, 0x0000023dd0723b20]
Event: 103.130 Thread 0x0000023de3ba1000 14219       3       org.eclipse.e4.ui.css.core.impl.sac.AbstractCombinatorCondition::getSpecificity (26 bytes)
Event: 103.131 Thread 0x0000023de3ba1000 nmethod 14219 0x0000023dd09b1ed0 code [0x0000023dd09b2060, 0x0000023dd09b2680]

GC Heap History (10 events):
Event: 38.437 GC heap before
{Heap before GC invocations=16 (full 1):
 par new generation   total 125120K, used 125120K [0x00000000c0000000, 0x00000000c8000000, 0x00000000c8000000)
  eden space 119168K, 100% used [0x00000000c0000000, 0x00000000c7460000, 0x00000000c7460000)
  from space 5952K, 100% used [0x00000000c7460000, 0x00000000c7a30000, 0x00000000c7a30000)
  to   space 5952K,   0% used [0x00000000c7a30000, 0x00000000c7a30000, 0x00000000c8000000)
 concurrent mark-sweep generation total 176128K, used 96059K [0x00000000c8000000, 0x00000000d2c00000, 0x0000000100000000)
 Metaspace       used 49422K, capacity 52623K, committed 52700K, reserved 1095680K
  class space    used 5273K, capacity 6098K, committed 6108K, reserved 1048576K
Event: 38.589 GC heap after
Heap after GC invocations=17 (full 1):
 par new generation   total 125120K, used 5952K [0x00000000c0000000, 0x00000000c8000000, 0x00000000c8000000)
  eden space 119168K,   0% used [0x00000000c0000000, 0x00000000c0000000, 0x00000000c7460000)
  from space 5952K, 100% used [0x00000000c7a30000, 0x00000000c8000000, 0x00000000c8000000)
  to   space 5952K,   0% used [0x00000000c7460000, 0x00000000c7460000, 0x00000000c7a30000)
 concurrent mark-sweep generation total 176128K, used 110384K [0x00000000c8000000, 0x00000000d2c00000, 0x0000000100000000)
 Metaspace       used 49422K, capacity 52623K, committed 52700K, reserved 1095680K
  class space    used 5273K, capacity 6098K, committed 6108K, reserved 1048576K
}
Event: 49.640 GC heap before
{Heap before GC invocations=17 (full 2):
 par new generation   total 125120K, used 125120K [0x00000000c0000000, 0x00000000c8000000, 0x00000000c8000000)
  eden space 119168K, 100% used [0x00000000c0000000, 0x00000000c7460000, 0x00000000c7460000)
  from space 5952K, 100% used [0x00000000c7a30000, 0x00000000c8000000, 0x00000000c8000000)
  to   space 5952K,   0% used [0x00000000c7460000, 0x00000000c7460000, 0x00000000c7a30000)
 concurrent mark-sweep generation total 176128K, used 43441K [0x00000000c8000000, 0x00000000d2c00000, 0x0000000100000000)
 Metaspace       used 62079K, capacity 66335K, committed 66440K, reserved 1107968K
  class space    used 7120K, capacity 8253K, committed 8328K, reserved 1048576K
Event: 49.693 GC heap after
Heap after GC invocations=18 (full 2):
 par new generation   total 125120K, used 5952K [0x00000000c0000000, 0x00000000c8000000, 0x00000000c8000000)
  eden space 119168K,   0% used [0x00000000c0000000, 0x00000000c0000000, 0x00000000c7460000)
  from space 5952K, 100% used [0x00000000c7460000, 0x00000000c7a30000, 0x00000000c7a30000)
  to   space 5952K,   0% used [0x00000000c7a30000, 0x00000000c7a30000, 0x00000000c8000000)
 concurrent mark-sweep generation total 176128K, used 59660K [0x00000000c8000000, 0x00000000d2c00000, 0x0000000100000000)
 Metaspace       used 62079K, capacity 66335K, committed 66440K, reserved 1107968K
  class space    used 7120K, capacity 8253K, committed 8328K, reserved 1048576K
}
Event: 51.289 GC heap before
{Heap before GC invocations=18 (full 2):
 par new generation   total 125120K, used 82727K [0x00000000c0000000, 0x00000000c8000000, 0x00000000c8000000)
  eden space 119168K,  64% used [0x00000000c0000000, 0x00000000c4af9c98, 0x00000000c7460000)
  from space 5952K, 100% used [0x00000000c7460000, 0x00000000c7a30000, 0x00000000c7a30000)
  to   space 5952K,   0% used [0x00000000c7a30000, 0x00000000c7a30000, 0x00000000c8000000)
 concurrent mark-sweep generation total 176128K, used 59660K [0x00000000c8000000, 0x00000000d2c00000, 0x0000000100000000)
 Metaspace       used 65654K, capacity 70339K, committed 70408K, reserved 1110016K
  class space    used 7591K, capacity 8918K, committed 8968K, reserved 1048576K
Event: 51.329 GC heap after
Heap after GC invocations=19 (full 2):
 par new generation   total 125120K, used 5951K [0x00000000c0000000, 0x00000000c8000000, 0x00000000c8000000)
  eden space 119168K,   0% used [0x00000000c0000000, 0x00000000c0000000, 0x00000000c7460000)
  from space 5952K,  99% used [0x00000000c7a30000, 0x00000000c7fffff8, 0x00000000c8000000)
  to   space 5952K,   0% used [0x00000000c7460000, 0x00000000c7460000, 0x00000000c7a30000)
 concurrent mark-sweep generation total 176128K, used 65915K [0x00000000c8000000, 0x00000000d2c00000, 0x0000000100000000)
 Metaspace       used 65654K, capacity 70339K, committed 70408K, reserved 1110016K
  class space    used 7591K, capacity 8918K, committed 8968K, reserved 1048576K
}
Event: 57.199 GC heap before
{Heap before GC invocations=19 (full 2):
 par new generation   total 125120K, used 125119K [0x00000000c0000000, 0x00000000c8000000, 0x00000000c8000000)
  eden space 119168K, 100% used [0x00000000c0000000, 0x00000000c7460000, 0x00000000c7460000)
  from space 5952K,  99% used [0x00000000c7a30000, 0x00000000c7fffff8, 0x00000000c8000000)
  to   space 5952K,   0% used [0x00000000c7460000, 0x00000000c7460000, 0x00000000c7a30000)
 concurrent mark-sweep generation total 176128K, used 65915K [0x00000000c8000000, 0x00000000d2c00000, 0x0000000100000000)
 Metaspace       used 70903K, capacity 76527K, committed 76552K, reserved 1116160K
  class space    used 8269K, capacity 9734K, committed 9736K, reserved 1048576K
Event: 57.267 GC heap after
Heap after GC invocations=20 (full 2):
 par new generation   total 125120K, used 5952K [0x00000000c0000000, 0x00000000c8000000, 0x00000000c8000000)
  eden space 119168K,   0% used [0x00000000c0000000, 0x00000000c0000000, 0x00000000c7460000)
  from space 5952K, 100% used [0x00000000c7460000, 0x00000000c7a30000, 0x00000000c7a30000)
  to   space 5952K,   0% used [0x00000000c7a30000, 0x00000000c7a30000, 0x00000000c8000000)
 concurrent mark-sweep generation total 176128K, used 81905K [0x00000000c8000000, 0x00000000d2c00000, 0x0000000100000000)
 Metaspace       used 70903K, capacity 76527K, committed 76552K, reserved 1116160K
  class space    used 8269K, capacity 9734K, committed 9736K, reserved 1048576K
}
Event: 67.887 GC heap before
{Heap before GC invocations=20 (full 2):
 par new generation   total 125120K, used 125120K [0x00000000c0000000, 0x00000000c8000000, 0x00000000c8000000)
  eden space 119168K, 100% used [0x00000000c0000000, 0x00000000c7460000, 0x00000000c7460000)
  from space 5952K, 100% used [0x00000000c7460000, 0x00000000c7a30000, 0x00000000c7a30000)
  to   space 5952K,   0% used [0x00000000c7a30000, 0x00000000c7a30000, 0x00000000c8000000)
 concurrent mark-sweep generation total 176128K, used 81905K [0x00000000c8000000, 0x00000000d2c00000, 0x0000000100000000)
 Metaspace       used 87425K, capacity 93925K, committed 94216K, reserved 1130496K
  class space    used 10468K, capacity 12170K, committed 12296K, reserved 1048576K
Event: 67.971 GC heap after
Heap after GC invocations=21 (full 2):
 par new generation   total 125120K, used 5952K [0x00000000c0000000, 0x00000000c8000000, 0x00000000c8000000)
  eden space 119168K,   0% used [0x00000000c0000000, 0x00000000c0000000, 0x00000000c7460000)
  from space 5952K, 100% used [0x00000000c7a30000, 0x00000000c8000000, 0x00000000c8000000)
  to   space 5952K,   0% used [0x00000000c7460000, 0x00000000c7460000, 0x00000000c7a30000)
 concurrent mark-sweep generation total 176128K, used 94671K [0x00000000c8000000, 0x00000000d2c00000, 0x0000000100000000)
 Metaspace       used 87425K, capacity 93925K, committed 94216K, reserved 1130496K
  class space    used 10468K, capacity 12170K, committed 12296K, reserved 1048576K
}

Deoptimization events (10 events):
Event: 82.039 Thread 0x0000023dc8e85800 Uncommon trap: reason=unstable_if action=reinterpret pc=0x0000023dd1974ed0 method=java.util.regex.Pattern.matcher(Ljava/lang/CharSequence;)Ljava/util/regex/Matcher; @ 4
Event: 82.039 Thread 0x0000023dc8e85800 Uncommon trap: reason=unstable_if action=reinterpret pc=0x0000023dd19f13d4 method=java.util.regex.Pattern.sequence(Ljava/util/regex/Pattern$Node;)Ljava/util/regex/Pattern$Node; @ 536
Event: 82.235 Thread 0x0000023dc8e85800 Uncommon trap: reason=unstable_if action=reinterpret pc=0x0000023dd0938dc4 method=java.lang.ThreadLocal$ThreadLocalMap.set(Ljava/lang/ThreadLocal;Ljava/lang/Object;)V @ 119
Event: 82.443 Thread 0x0000023dc8e85800 Uncommon trap: reason=unstable_if action=reinterpret pc=0x0000023dd166469c method=java.lang.AbstractStringBuilder.setLength(I)V @ 23
Event: 82.610 Thread 0x0000023dc8e85800 Uncommon trap: reason=unstable_if action=reinterpret pc=0x0000023dd0aff218 method=java.util.Hashtable.get(Ljava/lang/Object;)Ljava/lang/Object; @ 48
Event: 82.611 Thread 0x0000023dc8e85800 Uncommon trap: reason=class_check action=maybe_recompile pc=0x0000023dd06b111c method=java.util.Hashtable.put(Ljava/lang/Object;Ljava/lang/Object;)Ljava/lang/Object; @ 60
Event: 82.770 Thread 0x0000023deb3c8000 Uncommon trap: reason=unloaded action=reinterpret pc=0x0000023dd2385634 method=org.eclipse.ui.internal.UISynchronizer.syncExec(Ljava/lang/Runnable;)V @ 95
Event: 83.367 Thread 0x0000023dc8e85800 Uncommon trap: reason=unstable_if action=reinterpret pc=0x0000023dd06903a8 method=java.util.concurrent.locks.AbstractQueuedSynchronizer.doReleaseShared()V @ 69
Event: 88.538 Thread 0x0000023dc8e85800 Uncommon trap: reason=class_check action=maybe_recompile pc=0x0000023dd0c5b6ac method=org.eclipse.swt.widgets.Control.windowProc(JIJJ)J @ 1230
Event: 89.480 Thread 0x0000023dc8e85800 Uncommon trap: reason=unstable_if action=reinterpret pc=0x0000023dd05d8608 method=org.eclipse.swt.widgets.Display.filterMessage(Lorg/eclipse/swt/internal/win32/MSG;)Z @ 16

Classes redefined (0 events):
No events

Internal exceptions (10 events):
Event: 66.776 Thread 0x0000023deb3c8000 Exception <a 'java/lang/ClassNotFoundException': javax/servlet/ServletContext> (0x00000000c697d3a0) thrown at [C:\jenkins\workspace\8-2-build-windows-amd64-cygwin\jdk8u291\1294\hotspot\src\share\vm\classfile\systemDictionary.cpp, line 212]
Event: 67.113 Thread 0x0000023deb3c8000 Exception <a 'java/lang/ClassNotFoundException': com/sun/org/glassfish/hk2/osgiresourcelocator/ServiceLoader> (0x00000000c6e501a8) thrown at [C:\jenkins\workspace\8-2-build-windows-amd64-cygwin\jdk8u291\1294\hotspot\src\share\vm\classfile\systemDictionary
Event: 81.407 Thread 0x0000023dc8e85800 Exception <a 'java/io/FileNotFoundException'> (0x00000000c0be0378) thrown at [C:\jenkins\workspace\8-2-build-windows-amd64-cygwin\jdk8u291\1294\hotspot\src\share\vm\prims\jni.cpp, line 710]
Event: 81.420 Thread 0x0000023dc8e85800 Exception <a 'java/io/FileNotFoundException'> (0x00000000c0bf9cb8) thrown at [C:\jenkins\workspace\8-2-build-windows-amd64-cygwin\jdk8u291\1294\hotspot\src\share\vm\prims\jni.cpp, line 710]
Event: 82.264 Thread 0x0000023dc8e85800 Exception <a 'java/lang/ClassNotFoundException': br/com/germantech/ecf/dominio/modelo/balanca/BalancaBeanInfo> (0x00000000c16aba70) thrown at [C:\jenkins\workspace\8-2-build-windows-amd64-cygwin\jdk8u291\1294\hotspot\src\share\vm\classfile\systemDictionar
Event: 82.265 Thread 0x0000023dc8e85800 Exception <a 'java/lang/ClassNotFoundException': br/com/germantech/ecf/dominio/modelo/balanca/BalancaCustomizer> (0x00000000c16ba5d8) thrown at [C:\jenkins\workspace\8-2-build-windows-amd64-cygwin\jdk8u291\1294\hotspot\src\share\vm\classfile\systemDiction
Event: 82.333 Thread 0x0000023dc8e85800 Exception <a 'java/lang/ClassNotFoundException': br/com/germantech/ecf/dominio/compartilhado/LogBeanInfo> (0x00000000c17d2250) thrown at [C:\jenkins\workspace\8-2-build-windows-amd64-cygwin\jdk8u291\1294\hotspot\src\share\vm\classfile\systemDictionary.cpp
Event: 82.334 Thread 0x0000023dc8e85800 Exception <a 'java/lang/ClassNotFoundException': br/com/germantech/ecf/dominio/compartilhado/LogCustomizer> (0x00000000c17e0518) thrown at [C:\jenkins\workspace\8-2-build-windows-amd64-cygwin\jdk8u291\1294\hotspot\src\share\vm\classfile\systemDictionary.c
Event: 82.488 Thread 0x0000023dc8e85800 Exception <a 'java/lang/ClassNotFoundException': br/com/germantech/ecf/dominio/modelo/usuario/UsuarioBeanInfo> (0x00000000c1b07d08) thrown at [C:\jenkins\workspace\8-2-build-windows-amd64-cygwin\jdk8u291\1294\hotspot\src\share\vm\classfile\systemDictionar
Event: 82.489 Thread 0x0000023dc8e85800 Exception <a 'java/lang/ClassNotFoundException': br/com/germantech/ecf/dominio/modelo/usuario/UsuarioCustomizer> (0x00000000c1b16878) thrown at [C:\jenkins\workspace\8-2-build-windows-amd64-cygwin\jdk8u291\1294\hotspot\src\share\vm\classfile\systemDiction

Events (10 events):
Event: 89.507 loading class org/eclipse/core/internal/databinding/property/value/SimplePropertyObservableValue
Event: 89.507 loading class org/eclipse/core/internal/databinding/property/value/SimplePropertyObservableValue done
Event: 92.185 loading class org/eclipse/swt/widgets/Display
Event: 92.185 loading class org/eclipse/swt/widgets/Display done
Event: 92.185 loading class org/eclipse/jface/util/OpenStrategy$1
Event: 92.186 loading class org/eclipse/jface/util/OpenStrategy$1 done
Event: 103.043 Thread 0x0000023de3ba1000 flushing nmethod 0x0000023dd03b7f10
Event: 103.063 Thread 0x0000023de3ba1000 flushing nmethod 0x0000023dd0723750
Event: 103.108 Thread 0x0000023de3ba1000 flushing nmethod 0x0000023dd0aea310
Event: 103.129 Thread 0x0000023de3ba1000 flushing nmethod 0x0000023dd0ecc4d0


Dynamic libraries:
0x00007ff79f1b0000 - 0x00007ff79f1f7000 	C:\Program Files\Java\jre1.8.0_291\bin\javaw.exe
0x00007ff802790000 - 0x00007ff802b8f000 	C:\Windows\SYSTEM32\ntdll.dll
0x00007ff800210000 - 0x00007ff80030d000 	C:\Windows\System32\xtajit64.dll
0x00007ff801cf0000 - 0x00007ff801e51000 	C:\Windows\System32\KERNEL32.DLL
0x00007ffffded0000 - 0x00007ffffe502000 	C:\Windows\System32\KERNELBASE.dll
0x00007ffffd8c0000 - 0x00007ffffd9b1000 	C:\Windows\SYSTEM32\apphelp.dll
0x00007ff801bb0000 - 0x00007ff801ce7000 	C:\Windows\System32\ADVAPI32.dll
0x00007ff800310000 - 0x00007ff800454000 	C:\Windows\System32\msvcrt.dll
0x00007ff801030000 - 0x00007ff801157000 	C:\Windows\System32\sechost.dll
0x00007ff800560000 - 0x00007ff800780000 	C:\Windows\System32\RPCRT4.dll
0x00007ff801170000 - 0x00007ff8013ce000 	C:\Windows\System32\USER32.dll
0x00007ffffe510000 - 0x00007ffffe56c000 	C:\Windows\System32\win32u.dll
0x00007ff800ea0000 - 0x00007ff800efa000 	C:\Windows\System32\GDI32.dll
0x00007ffffea00000 - 0x00007ffffebe3000 	C:\Windows\System32\gdi32full.dll
0x00007ffffe6b0000 - 0x00007ffffe7f3000 	C:\Windows\System32\msvcp_win.dll
0x00007ffffe800000 - 0x00007ffffe9f1000 	C:\Windows\System32\ucrtbase.dll
0x00007fffe63b0000 - 0x00007fffe6822000 	C:\Windows\WinSxS\arm64_microsoft.windows.common-controls_6595b64144ccf1df_6.0.22621.1344_none_2710876173851695\COMCTL32.dll
0x00007ff800000000 - 0x00007ff800052000 	C:\Windows\System32\IMM32.DLL
0x00007fffec290000 - 0x00007fffec2a5000 	C:\Program Files\Java\jre1.8.0_291\bin\vcruntime140.dll
0x00007fffddd00000 - 0x00007fffddd9b000 	C:\Program Files\Java\jre1.8.0_291\bin\msvcp140.dll
0x0000000008000000 - 0x0000000008860000 	C:\Program Files\Java\jre1.8.0_291\bin\server\jvm.dll
0x00007ff800460000 - 0x00007ff80046e000 	C:\Windows\System32\PSAPI.DLL
0x00007fffdea30000 - 0x00007fffdea42000 	C:\Windows\SYSTEM32\WSOCK32.dll
0x00007ffff2c40000 - 0x00007ffff2c9e000 	C:\Windows\SYSTEM32\WINMM.dll
0x00007fffe8400000 - 0x00007fffe8415000 	C:\Windows\SYSTEM32\VERSION.dll
0x00007ffffecc0000 - 0x00007ffffed84000 	C:\Windows\System32\WS2_32.dll
0x00007ffffc130000 - 0x00007ffffc15d000 	C:\Windows\SYSTEM32\kernel.appcore.dll
0x00007ffff4440000 - 0x00007ffff4450000 	C:\Program Files\Java\jre1.8.0_291\bin\verify.dll
0x00007fffde250000 - 0x00007fffde27b000 	C:\Program Files\Java\jre1.8.0_291\bin\java.dll
0x00007fffec010000 - 0x00007fffec028000 	C:\Program Files\Java\jre1.8.0_291\bin\zip.dll
0x00007fffff010000 - 0x00007ffffffec000 	C:\Windows\System32\SHELL32.dll
0x00007ffffa250000 - 0x00007ffffb565000 	C:\Windows\SYSTEM32\windows.storage.dll
0x00007ff8013d0000 - 0x00007ff801a75000 	C:\Windows\System32\combase.dll
0x00007ffff9fd0000 - 0x00007ffffa243000 	C:\Windows\SYSTEM32\wintypes.dll
0x00007ff800780000 - 0x00007ff800972000 	C:\Windows\System32\SHCORE.dll
0x00007ffffef60000 - 0x00007fffff007000 	C:\Windows\System32\shlwapi.dll
0x00007ffffdde0000 - 0x00007ffffde1b000 	C:\Windows\SYSTEM32\profapi.dll
0x00007ffffccb0000 - 0x00007ffffcce2000 	C:\Windows\SYSTEM32\CRYPTSP.dll
0x00007ffffc060000 - 0x00007ffffc0c3000 	C:\Windows\system32\rsaenh.dll
0x00007ffffc990000 - 0x00007ffffc9de000 	C:\Windows\SYSTEM32\USERENV.dll
0x00007ffffcf90000 - 0x00007ffffcfda000 	C:\Windows\SYSTEM32\bcrypt.dll
0x00007ffffebf0000 - 0x00007ffffecbb000 	C:\Windows\System32\bcryptprimitives.dll
0x00007ffffccf0000 - 0x00007ffffcd04000 	C:\Windows\SYSTEM32\CRYPTBASE.dll
0x00007fffeb1a0000 - 0x00007fffeb1bc000 	C:\Program Files\Java\jre1.8.0_291\bin\net.dll
0x00007ffffc7e0000 - 0x00007ffffc8a3000 	C:\Windows\system32\mswsock.dll
0x00007ffffb8c0000 - 0x00007ffffb913000 	C:\Windows\SYSTEM32\IPHLPAPI.DLL
0x00007ff802680000 - 0x00007ff802690000 	C:\Windows\System32\NSI.dll
0x00007ffff25e0000 - 0x00007ffff2608000 	C:\Windows\SYSTEM32\dhcpcsvc6.DLL
0x00007ffff2630000 - 0x00007ffff266c000 	C:\Windows\SYSTEM32\dhcpcsvc.DLL
0x00007ffffb960000 - 0x00007ffffbb11000 	C:\Windows\SYSTEM32\DNSAPI.dll
0x00007fffe0670000 - 0x00007fffe0683000 	C:\Program Files\Java\jre1.8.0_291\bin\nio.dll
0x00007fffd7d20000 - 0x00007fffd7d49000 	C:\Users\germantech-moroni\workspace-ecf\.metadata\.plugins\org.eclipse.pde.core\.bundle_pool\plugins\org.eclipse.equinox.launcher.win32.win32.x86_64_1.1.800.v20180827-1352\eclipse_1705.dll
0x00007ffff8e60000 - 0x00007ffff8f92000 	C:\Windows\system32\uxtheme.dll
0x00007ff800980000 - 0x00007ff800b8f000 	C:\Windows\System32\MSCTF.dll
0x00007fffef1c0000 - 0x00007fffef408000 	C:\Windows\SYSTEM32\textinputframework.dll
0x00007ff800060000 - 0x00007ff800201000 	C:\Windows\System32\OLEAUT32.dll
0x00007ffff8270000 - 0x00007ffff852a000 	C:\Windows\SYSTEM32\CoreMessaging.dll
0x00007ffff1be0000 - 0x00007ffff22ac000 	C:\Windows\SYSTEM32\CoreUIComponents.dll
0x00007fffa4cf0000 - 0x00007fffa4d91000 	C:\Users\germantech-moroni\workspace-ecf\.metadata\.plugins\org.eclipse.pde.core\br.com.germantech.product\org.eclipse.osgi\371\0\.cp\swt-win32-4919.dll
0x00007ff801e70000 - 0x00007ff80211f000 	C:\Windows\System32\ole32.dll
0x00007ffffed90000 - 0x00007ffffef56000 	C:\Windows\System32\COMDLG32.dll
0x00007fffde230000 - 0x00007fffde24c000 	C:\Windows\SYSTEM32\USP10.dll
0x00007fffe8fd0000 - 0x00007fffe90e0000 	C:\Windows\SYSTEM32\WINSPOOL.DRV
0x00007fffd6110000 - 0x00007fffd6851000 	C:\Windows\SYSTEM32\WININET.dll
0x00007ffffdb40000 - 0x00007ffffddd7000 	C:\Windows\SYSTEM32\CRYPT32.dll
0x00007ff801ad0000 - 0x00007ff801bae000 	C:\Windows\System32\coml2.dll
0x00007ffff9940000 - 0x00007ffff9b15000 	C:\Windows\SYSTEM32\propsys.dll
0x00007ff800f00000 - 0x00007ff801030000 	C:\Windows\System32\clbcatq.dll
0x00007fffcbb90000 - 0x00007fffcbf35000 	C:\Windows\System32\TaskFlowDataEngine.dll
0x00007fffde6c0000 - 0x00007fffde810000 	C:\Windows\System32\OneCoreCommonProxyStub.dll
0x00007fffd0770000 - 0x00007fffd0797000 	C:\Users\germantech-moroni\workspace-ecf\.metadata\.plugins\org.eclipse.pde.core\br.com.germantech.product\org.eclipse.osgi\371\0\.cp\swt-gdip-win32-4919.dll
0x00007fffbe9e0000 - 0x00007fffbece6000 	C:\Windows\WinSxS\arm64_microsoft.windows.gdiplus_6595b64144ccf1df_1.1.22621.819_none_da3042dd1b9d3f25\gdiplus.dll
0x00007ffff6300000 - 0x00007ffff6601000 	C:\Windows\SYSTEM32\WindowsCodecs.dll
0x00007ffff2ef0000 - 0x00007ffff2efd000 	C:\Program Files\Java\jre1.8.0_291\bin\management.dll
0x00007fffddfc0000 - 0x00007fffddfe4000 	C:\Program Files\Java\jre1.8.0_291\bin\sunec.dll
0x00007fffd8620000 - 0x00007fffd864c000 	C:\Windows\system32\napinsp.dll
0x00007fffd8280000 - 0x00007fffd82b3000 	C:\Windows\system32\pnrpnsp.dll
0x00007fffd82c0000 - 0x00007fffd82fe000 	C:\Windows\system32\nlansp_c.dll
0x00007fffd8260000 - 0x00007fffd8280000 	C:\Windows\System32\winrnr.dll
0x00007fffd83b0000 - 0x00007fffd83db000 	C:\Windows\system32\wshbth.dll
0x00007ffff02f0000 - 0x00007ffff03db000 	C:\Windows\System32\fwpuclnt.dll
0x00007ffff0a20000 - 0x00007ffff0a32000 	C:\Windows\System32\rasadhlp.dll
0x00007fffcf230000 - 0x00007fffcf2fc000 	C:\Windows\SYSTEM32\oleacc.dll
0x00007fffdefc0000 - 0x00007fffdf0c1000 	C:\Windows\SYSTEM32\TextShaping.dll
0x00007fffd9ca0000 - 0x00007fffd9cad000 	C:\Windows\SYSTEM32\msimg32.dll
0x00007fffdb760000 - 0x00007fffdb7cc000 	C:\Windows\system32\mlang.dll
0x00007fffcdc80000 - 0x00007fffce1a3000 	C:\Windows\system32\explorerframe.dll
0x00007fff7fc20000 - 0x00007fff7fdb5000 	C:\Program Files\Java\jre1.8.0_291\bin\awt.dll
0x00007ffff6610000 - 0x00007ffff6a77000 	C:\Windows\SYSTEM32\DWrite.dll
0x00007fffec340000 - 0x00007fffec34d000 	C:\Program Files\Java\jre1.8.0_291\bin\sunmscapi.dll
0x00007ffffcf30000 - 0x00007ffffcf83000 	C:\Windows\SYSTEM32\ncrypt.dll
0x00007ffffcec0000 - 0x00007ffffcf23000 	C:\Windows\SYSTEM32\NTASN1.dll
0x00007ffff95e0000 - 0x00007ffff962c000 	C:\Windows\system32\dwmapi.dll
0x0000000071100000 - 0x0000000071125000 	C:\Users\germantech-moroni\.jssc\windows\jSSC-2.8_x86_64.dll
0x00007fffe8b50000 - 0x00007fffe8f60000 	C:\Windows\SYSTEM32\dbghelp.dll

VM Arguments:
jvm_args: -Xms300m -Xmx1024m -Xmn128m -XX:SurvivorRatio=20 -XX:+UseConcMarkSweepGC -XX:+CMSParallelRemarkEnabled -XX:+UseParNewGC -Dfile.encoding=UTF8 -Dhttps.protocols=TLSv1.2 -Declipse.p2.unsignedPolicy=allow -Djava.net.preferIPv4Stack=true 
java_command: org.eclipse.equinox.launcher.Main -launcher C:\Users\germantech-moroni\workspace-ecf\.metadata\.plugins\org.eclipse.pde.core\.bundle_pool\eclipse.exe -name Eclipse -showsplash 600 -product br.com.germantech.ecf.br_com_germantech_core -data C:\Users\germantech-moroni\workspace-ecf/../runtime-br.com.germantech.product -configuration file:C:/Users/germantech-moroni/workspace-ecf/.metadata/.plugins/org.eclipse.pde.core/br.com.germantech.product/ -dev file:C:/Users/germantech-moroni/workspace-ecf/.metadata/.plugins/org.eclipse.pde.core/br.com.germantech.product/dev.properties -os win32 -ws win32 -arch x86_64 -nl en_US -consoleLog pt_BR -clean -clearPersistedState -vm jre8/bin/javaw.exe
java_class_path (initial): C:\Users\germantech-moroni\workspace-ecf\.metadata\.plugins\org.eclipse.pde.core\.bundle_pool\plugins\org.eclipse.equinox.launcher_1.5.100.v20180827-1352.jar
Launcher Type: SUN_STANDARD

Environment Variables:
PATH=C:\Program Files (x86)\Common Files\Oracle\Java\javapath;C:\Program Files\Parallels\Parallels Tools\Applications;C:\Windows\system32;C:\Windows;C:\Windows\System32\Wbem;C:\Windows\System32\WindowsPowerShell\v1.0\;C:\Windows\System32\OpenSSH\;C:\Program Files\Git\cmd;C:\Program Files\nodejs\;C:\Users\germantech-moroni\AppData\Local\Microsoft\WindowsApps;C:\Users\germantech-moroni\AppData\Local\GitHubDesktop\bin;C:\Users\germantech-moroni\AppData\Roaming\npm;C:\Users\germantech-moroni\AppData\Local\Programs\Microsoft VS Code\bin
USERNAME=germantech-moroni
OS=Windows_NT
PROCESSOR_IDENTIFIER=ARMv8 (64-bit) Family 8 Model 0 Revision   0,  



---------------  S Y S T E M  ---------------

OS: Windows 10.0 , 64 bit Build 22621 (10.0.22621.1485)

CPU:total 4 (initial active 4) (4 cores per cpu, 1 threads per core) family 15 model 4 stepping 10, cmov, cx8, fxsr, mmx, sse, sse2, sse3, ssse3, sse4.1, sse4.2, popcnt, aes, clmul, tsc, tscinvbit, tscinv

Memory: 4k page, physical 3140208k(429204k free), swap 7782536k(1430840k free)

vm_info: Java HotSpot(TM) 64-Bit Server VM (25.291-b10) for windows-amd64 JRE (1.8.0_291-b10), built on Apr  9 2021 00:02:00 by "java_re" with MS VC++ 15.9 (VS2017)

time: Mon May  8 17:47:26 2023
timezone: E. South America Standard Time
elapsed time: 103.231965 seconds (0d 0h 1m 43s)

