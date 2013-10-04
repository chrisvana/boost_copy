// Test
[
  { "config": {
    "component": "boost",
    "component_root": "boost"
  } },

  { "gen_sh": {
    "name": "boost_gen",
    "build_cmd": "toolset=\"clang\"; [ \"$CXX_GCC\" = 1 ] && toolset=gcc; ./bootstrap.sh && ./b2 toolset=\"$toolset\" cflags=\"-O3 $BASIC_CFLAGS\" cxxflags=\"-O3 $BASIC_CXXFLAGS\" threading=multi linkflags=\"$LDFLAGS\" -j8 --stagedir=\"$GEN_DIR\" && ([ ! -e $GEN_DIR/include ] && ln -f -s $(pwd) $GEN_DIR/include || echo -n '')",
    "clean": "./b2 clean",
    "outs": [ "lib/libboost_atomic.a",
              "lib/libboost_chrono.a",
              "lib/libboost_context.a",
              "lib/libboost_coroutine.a",
              "lib/libboost_date_time.a",
              "lib/libboost_exception.a",
              "lib/libboost_filesystem.a",
              "lib/libboost_graph.a",
              "lib/libboost_iostreams.a",
              "lib/libboost_log.a",
              "lib/libboost_log_setup.a",
              "lib/libboost_math_c99.a",
              "lib/libboost_math_c99f.a",
              "lib/libboost_math_c99l.a",
              "lib/libboost_math_tr1.a",
              "lib/libboost_math_tr1f.a",
              "lib/libboost_math_tr1l.a",
              "lib/libboost_prg_exec_monitor.a",
              "lib/libboost_program_options.a",
              "lib/libboost_python.a",
              "lib/libboost_random.a",
              "lib/libboost_regex.a",
              "lib/libboost_serialization.a",
              "lib/libboost_signals.a",
              "lib/libboost_system.a",
              "lib/libboost_test_exec_monitor.a",
              "lib/libboost_thread.a",
              "lib/libboost_timer.a",
              "lib/libboost_unit_test_framework.a",
              "lib/libboost_wave.a",
              "lib/libboost_wserialization.a"
    ],
    "env" : {
      "BOOST_ROOT" : "$GEN_DIR",
      "BOOST_INCLUDEDIR" : "$SRC_DIR",
      "BOOST_LIBDIR" : "$GEN_DIR/lib"
    }
  } },

  { "cc_library": {
    "name": "boost_headers"
    // Unless you are developing boost, you don't need this. Commented out
    // for speed.
    //"cc_headers": [ "boost/*.hpp",
    //                "boost/*/*.hpp",
    //                "boost/*/*/*.hpp",
    //                "boost/*/*/*/*.hpp",
    //                "boost/*/*/*/*/*.hpp",
    //                "boost/*/*/*/*/*/*.hpp",
    //                "boost/*/*/*/*/*/*/*.hpp",
    //                "boost/*/*/*/*/*/*/*/*.hpp"
    //]
  } },

  { "cc_library": {
    "name": "atomic",
    "cc_objects": [ "$GEN_DIR/lib/libboost_atomic.a" ],
    "strict_file_mode": false,
    "dependencies": [ ":boost_gen", ":boost_headers" ]
  } },
  { "cc_library": {
    "name": "chrono",
    "cc_objects": [ "$GEN_DIR/lib/libboost_chrono.a" ],
    "strict_file_mode": false,
    "dependencies": [ ":boost_gen", ":boost_headers" ]
  } },
  { "cc_library": {
    "name": "context",
    "cc_objects": [ "$GEN_DIR/lib/libboost_context.a" ],
    "strict_file_mode": false,
    "dependencies": [ ":boost_gen", ":boost_headers" ]
  } },
  { "cc_library": {
    "name": "coroutine",
    "cc_objects": [ "$GEN_DIR/lib/libboost_coroutine.a" ],
    "strict_file_mode": false,
    "dependencies": [ ":boost_gen", ":boost_headers" ]
  } },
  { "cc_library": {
    "name": "date_time",
    "cc_objects": [ "$GEN_DIR/lib/libboost_date_time.a" ],
    "strict_file_mode": false,
    "dependencies": [ ":boost_gen", ":boost_headers" ]
  } },
  { "cc_library": {
    "name": "exception",
    "cc_objects": [ "$GEN_DIR/lib/libboost_exception.a" ],
    "strict_file_mode": false,
    "dependencies": [ ":boost_gen", ":boost_headers" ]
  } },
  { "cc_library": {
    "name": "filesystem",
    "cc_objects": [ "$GEN_DIR/lib/libboost_filesystem.a" ],
    "strict_file_mode": false,
    "dependencies": [ ":boost_gen", ":boost_headers" ]
  } },
  { "cc_library": {
    "name": "graph",
    "cc_objects": [ "$GEN_DIR/lib/libboost_graph.a" ],
    "strict_file_mode": false,
    "dependencies": [ ":boost_gen", ":boost_headers" ]
  } },
  { "cc_library": {
    "name": "iostreams",
    "cc_objects": [ "$GEN_DIR/lib/libboost_iostreams.a" ],
    "strict_file_mode": false,
    "dependencies": [ ":boost_gen", ":boost_headers" ]
  } },
  { "cc_library": {
    "name": "log",
    "cc_objects": [ "$GEN_DIR/lib/libboost_log.a" ],
    "strict_file_mode": false,
    "dependencies": [ ":boost_gen", ":boost_headers" ]
  } },
  { "cc_library": {
    "name": "log_setup",
    "cc_objects": [ "$GEN_DIR/lib/libboost_log_setup.a" ],
    "strict_file_mode": false,
    "dependencies": [ ":boost_gen", ":boost_headers" ]
  } },
  { "cc_library": {
    "name": "math_c99",
    "cc_objects": [ "$GEN_DIR/lib/libboost_math_c99.a" ],
    "strict_file_mode": false,
    "dependencies": [ ":boost_gen", ":boost_headers" ]
  } },
  { "cc_library": {
    "name": "math_c99f",
    "cc_objects": [ "$GEN_DIR/lib/libboost_math_c99f.a" ],
    "strict_file_mode": false,
    "dependencies": [ ":boost_gen", ":boost_headers" ]
  } },
  { "cc_library": {
    "name": "math_c99l",
    "cc_objects": [ "$GEN_DIR/lib/libboost_math_c99l.a" ],
    "strict_file_mode": false,
    "dependencies": [ ":boost_gen", ":boost_headers" ]
  } },
  { "cc_library": {
    "name": "math_tr1",
    "cc_objects": [ "$GEN_DIR/lib/libboost_math_tr1.a" ],
    "strict_file_mode": false,
    "dependencies": [ ":boost_gen", ":boost_headers" ]
  } },
  { "cc_library": {
    "name": "math_tr1f",
    "cc_objects": [ "$GEN_DIR/lib/libboost_math_tr1f.a" ],
    "strict_file_mode": false,
    "dependencies": [ ":boost_gen", ":boost_headers" ]
  } },
  { "cc_library": {
    "name": "math_tr1l",
    "cc_objects": [ "$GEN_DIR/lib/libboost_math_tr1l.a" ],
    "strict_file_mode": false,
    "dependencies": [ ":boost_gen", ":boost_headers" ]
  } },
  { "cc_library": {
    "name": "prg_exec_monitor",
    "cc_objects": [ "$GEN_DIR/lib/libboost_prg_exec_monitor.a" ],
    "strict_file_mode": false,
    "dependencies": [ ":boost_gen", ":boost_headers" ]
  } },
  { "cc_library": {
    "name": "program_options",
    "cc_objects": [ "$GEN_DIR/lib/libboost_program_options.a" ],
    "strict_file_mode": false,
    "dependencies": [ ":boost_gen", ":boost_headers" ]
  } },
  { "cc_library": {
    "name": "python",
    "cc_objects": [ "$GEN_DIR/lib/libboost_python.a" ],
    "strict_file_mode": false,
    "dependencies": [ ":boost_gen", ":boost_headers" ]
  } },
  { "cc_library": {
    "name": "random",
    "cc_objects": [ "$GEN_DIR/lib/libboost_random.a" ],
    "strict_file_mode": false,
    "dependencies": [ ":boost_gen", ":boost_headers" ]
  } },
  { "cc_library": {
    "name": "regex",
    "cc_objects": [ "$GEN_DIR/lib/libboost_regex.a" ],
    "strict_file_mode": false,
    "dependencies": [ ":boost_gen", ":boost_headers" ]
  } },
  { "cc_library": {
    "name": "serialization",
    "cc_objects": [ "$GEN_DIR/lib/libboost_serialization.a" ],
    "strict_file_mode": false,
    "dependencies": [ ":boost_gen", ":boost_headers" ]
  } },
  { "cc_library": {
    "name": "signals",
    "cc_objects": [ "$GEN_DIR/lib/libboost_signals.a" ],
    "strict_file_mode": false,
    "dependencies": [ ":boost_gen", ":boost_headers" ]
  } },
  { "cc_library": {
    "name": "system",
    "cc_objects": [ "$GEN_DIR/lib/libboost_system.a" ],
    "strict_file_mode": false,
    "dependencies": [ ":boost_gen", ":boost_headers" ]
  } },
  { "cc_library": {
    "name": "test_exec_monitor",
    "cc_objects": [ "$GEN_DIR/lib/libboost_test_exec_monitor.a" ],
    "strict_file_mode": false,
    "dependencies": [ ":boost_gen", ":boost_headers" ]
  } },
  { "cc_library": {
    "name": "thread",
    "cc_objects": [ "$GEN_DIR/lib/libboost_thread.a" ],
    "strict_file_mode": false,
    "dependencies": [ ":boost_gen", ":boost_headers" ]
  } },
  { "cc_library": {
    "name": "timer",
    "cc_objects": [ "$GEN_DIR/lib/libboost_timer.a" ],
    "strict_file_mode": false,
    "dependencies": [ ":boost_gen", ":boost_headers" ]
  } },
  { "cc_library": {
    "name": "unit_test_framework",
    "cc_objects": [ "$GEN_DIR/lib/libboost_unit_test_framework.a" ],
    "strict_file_mode": false,
    "dependencies": [ ":boost_gen", ":boost_headers" ]
  } },
  { "cc_library": {
    "name": "wave",
    "cc_objects": [ "$GEN_DIR/lib/libboost_wave.a" ],
    "strict_file_mode": false,
    "dependencies": [ ":boost_gen", ":boost_headers" ]
  } },
  { "cc_library": {
    "name": "wserialization",
    "cc_objects": [ "$GEN_DIR/lib/libboost_wserialization.a" ],
    "strict_file_mode": false,
    "dependencies": [ ":boost_gen", ":boost_headers" ]
  } },
  { "cc_library": {
    "name": "boost",    
    "cc_objects": [ "$GEN_DIR/lib/libboost_atomic.a",
                    "$GEN_DIR/lib/libboost_chrono.a",
                    "$GEN_DIR/lib/libboost_context.a",
                    "$GEN_DIR/lib/libboost_coroutine.a",
                    "$GEN_DIR/lib/libboost_date_time.a",
                    "$GEN_DIR/lib/libboost_exception.a",
                    "$GEN_DIR/lib/libboost_filesystem.a",
                    "$GEN_DIR/lib/libboost_graph.a",
                    "$GEN_DIR/lib/libboost_iostreams.a",
                    "$GEN_DIR/lib/libboost_log.a",
                    "$GEN_DIR/lib/libboost_log_setup.a",
                    "$GEN_DIR/lib/libboost_math_c99.a",
                    "$GEN_DIR/lib/libboost_math_c99f.a",
                    "$GEN_DIR/lib/libboost_math_c99l.a",
                    "$GEN_DIR/lib/libboost_math_tr1.a",
                    "$GEN_DIR/lib/libboost_math_tr1f.a",
                    "$GEN_DIR/lib/libboost_math_tr1l.a",
                    "$GEN_DIR/lib/libboost_prg_exec_monitor.a",
                    "$GEN_DIR/lib/libboost_program_options.a",
                    "$GEN_DIR/lib/libboost_python.a",
                    "$GEN_DIR/lib/libboost_random.a",
                    "$GEN_DIR/lib/libboost_regex.a",
                    "$GEN_DIR/lib/libboost_serialization.a",
                    "$GEN_DIR/lib/libboost_signals.a",
                    "$GEN_DIR/lib/libboost_system.a",
                    "$GEN_DIR/lib/libboost_test_exec_monitor.a",
                    "$GEN_DIR/lib/libboost_thread.a",
                    "$GEN_DIR/lib/libboost_timer.a",
                    "$GEN_DIR/lib/libboost_unit_test_framework.a",
                    "$GEN_DIR/lib/libboost_wave.a",
                    "$GEN_DIR/lib/libboost_wserialization.a"
    ],
    "strict_file_mode": false,
    "dependencies": [ ":boost_gen", ":boost_headers" ]
  } }
]