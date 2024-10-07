diff --git a/platforms/osx/build_framework.py b/platforms/osx/build_framework.py
index 2dd5015..03e2155 100644
--- a/platforms/osx/build_framework.py
+++ b/platforms/osx/build_framework.py
@@ -78,6 +78,8 @@ if __name__ == "__main__":
     parser.add_argument('--run_tests', default=False, dest='run_tests', action='store_true', help='Run tests')
     parser.add_argument('--build_docs', default=False, dest='build_docs', action='store_true', help='Build docs')
     parser.add_argument('--disable-swift', default=False, dest='swiftdisabled', action='store_true', help='Disable building of Swift extensions')
+    parser.add_argument('--extra_cmake_options', default='', help='Extra options to pass to CMake')
+
 
     args, unknown_args = parser.parse_known_args()
     if unknown_args:
@@ -128,5 +130,5 @@ if __name__ == "__main__":
     if catalyst_archs:
         targets.append((catalyst_archs, "Catalyst")),
 
-    b = OSXBuilder(args.opencv, args.contrib, args.dynamic, True, args.without, args.disable, args.enablenonfree, targets, args.debug, args.debug_info, args.framework_name, args.run_tests, args.build_docs, args.swiftdisabled)
+    b = OSXBuilder(args.opencv, args.contrib, args.dynamic, True, args.without, args.disable, args.enablenonfree, targets, args.debug, args.debug_info, args.framework_name, args.run_tests, args.build_docs, args.swiftdisabled, args.extra_cmake_options)
     b.build(args.out)
