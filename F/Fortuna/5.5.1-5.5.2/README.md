# Comparing `tmp/fortuna-5.5.1.tar.gz` & `tmp/fortuna-5.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fortuna-5.5.1.tar", last modified: Sun Apr 28 16:33:29 2024, max compression
+gzip compressed data, was "fortuna-5.5.2.tar", last modified: Tue May 14 22:17:44 2024, max compression
```

## Comparing `fortuna-5.5.1.tar` & `fortuna-5.5.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 SpiritHome   (503) staff       (20)        0 2024-04-28 16:33:29.247418 fortuna-5.5.1/
--rw-r--r--   0 SpiritHome   (503) staff       (20)  1694227 2024-04-28 16:33:29.000000 fortuna-5.5.1/Fortuna.cpp
-drwxr-xr-x   0 SpiritHome   (503) staff       (20)        0 2024-04-28 16:33:29.246690 fortuna-5.5.1/Fortuna.egg-info/
--rw-r--r--   0 SpiritHome   (503) staff       (20)   112905 2024-04-28 16:33:29.000000 fortuna-5.5.1/Fortuna.egg-info/PKG-INFO
--rw-r--r--   0 SpiritHome   (503) staff       (20)      241 2024-04-28 16:33:29.000000 fortuna-5.5.1/Fortuna.egg-info/SOURCES.txt
--rw-r--r--   0 SpiritHome   (503) staff       (20)        1 2024-04-28 16:33:29.000000 fortuna-5.5.1/Fortuna.egg-info/dependency_links.txt
--rw-r--r--   0 SpiritHome   (503) staff       (20)       28 2024-04-28 16:33:29.000000 fortuna-5.5.1/Fortuna.egg-info/requires.txt
--rw-r--r--   0 SpiritHome   (503) staff       (20)        8 2024-04-28 16:33:29.000000 fortuna-5.5.1/Fortuna.egg-info/top_level.txt
--rw-r--r--   0 SpiritHome   (503) staff       (20)    35969 2024-04-28 16:32:06.000000 fortuna-5.5.1/Fortuna.pyx
--rw-r--r--   0 SpiritHome   (503) staff       (20)    18502 2018-12-08 18:44:55.000000 fortuna-5.5.1/LICENSE
--rw-r--r--   0 SpiritHome   (503) staff       (20)       72 2020-02-25 22:03:43.000000 fortuna-5.5.1/MANIFEST.in
--rw-r--r--   0 SpiritHome   (503) staff       (20)   112905 2024-04-28 16:33:29.247137 fortuna-5.5.1/PKG-INFO
--rw-r--r--   0 SpiritHome   (503) staff       (20)   111540 2024-02-29 20:28:19.000000 fortuna-5.5.1/README.md
--rw-r--r--   0 SpiritHome   (503) staff       (20)    20871 2024-04-06 22:59:20.000000 fortuna-5.5.1/Storm.hpp
--rw-r--r--   0 SpiritHome   (503) staff       (20)       60 2022-09-17 22:40:25.000000 fortuna-5.5.1/pyproject.toml
--rw-r--r--   0 SpiritHome   (503) staff       (20)       38 2024-04-28 16:33:29.247464 fortuna-5.5.1/setup.cfg
--rw-r--r--   0 SpiritHome   (503) staff       (20)     2480 2024-04-24 22:38:39.000000 fortuna-5.5.1/setup.py
+drwxr-xr-x   0 SpiritHome   (503) staff       (20)        0 2024-05-14 22:17:44.369830 fortuna-5.5.2/
+-rw-r--r--   0 SpiritHome   (503) staff       (20)  1725879 2024-05-14 22:17:44.000000 fortuna-5.5.2/Fortuna.cpp
+drwxr-xr-x   0 SpiritHome   (503) staff       (20)        0 2024-05-14 22:17:44.369150 fortuna-5.5.2/Fortuna.egg-info/
+-rw-r--r--   0 SpiritHome   (503) staff       (20)    85163 2024-05-14 22:17:44.000000 fortuna-5.5.2/Fortuna.egg-info/PKG-INFO
+-rw-r--r--   0 SpiritHome   (503) staff       (20)      241 2024-05-14 22:17:44.000000 fortuna-5.5.2/Fortuna.egg-info/SOURCES.txt
+-rw-r--r--   0 SpiritHome   (503) staff       (20)        1 2024-05-14 22:17:44.000000 fortuna-5.5.2/Fortuna.egg-info/dependency_links.txt
+-rw-r--r--   0 SpiritHome   (503) staff       (20)       28 2024-05-14 22:17:44.000000 fortuna-5.5.2/Fortuna.egg-info/requires.txt
+-rw-r--r--   0 SpiritHome   (503) staff       (20)        8 2024-05-14 22:17:44.000000 fortuna-5.5.2/Fortuna.egg-info/top_level.txt
+-rw-r--r--   0 SpiritHome   (503) staff       (20)    36566 2024-05-03 05:06:36.000000 fortuna-5.5.2/Fortuna.pyx
+-rw-r--r--   0 SpiritHome   (503) staff       (20)    18502 2018-12-08 18:44:55.000000 fortuna-5.5.2/LICENSE
+-rw-r--r--   0 SpiritHome   (503) staff       (20)       72 2020-02-25 22:03:43.000000 fortuna-5.5.2/MANIFEST.in
+-rw-r--r--   0 SpiritHome   (503) staff       (20)    85163 2024-05-14 22:17:44.369592 fortuna-5.5.2/PKG-INFO
+-rw-r--r--   0 SpiritHome   (503) staff       (20)    83798 2024-05-14 21:56:32.000000 fortuna-5.5.2/README.md
+-rw-r--r--   0 SpiritHome   (503) staff       (20)    19161 2024-05-14 22:17:12.000000 fortuna-5.5.2/Storm.hpp
+-rw-r--r--   0 SpiritHome   (503) staff       (20)       60 2022-09-17 22:40:25.000000 fortuna-5.5.2/pyproject.toml
+-rw-r--r--   0 SpiritHome   (503) staff       (20)       38 2024-05-14 22:17:44.369878 fortuna-5.5.2/setup.cfg
+-rw-r--r--   0 SpiritHome   (503) staff       (20)     2480 2024-05-14 21:54:44.000000 fortuna-5.5.2/setup.py
```

### Comparing `fortuna-5.5.1/Fortuna.cpp` & `fortuna-5.5.2/Fortuna.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -1575,15 +1575,15 @@
 struct __pyx_obj_7Fortuna___pyx_scope_struct__truffle_shuffle {
   PyObject_HEAD
   PyObject *__pyx_v_data;
   PyObject *__pyx_v_rotate_size;
 };
 
 
-/* "Fortuna.pyx":845
+/* "Fortuna.pyx":860
  *             w_pair[0] = cum_weight
  *         self.max_weight = optimized_data[-1][0]
  *         self.data = tuple(tuple(itm) for itm in optimized_data)             # <<<<<<<<<<<<<<
  * 
  * 
  */
 struct __pyx_obj_7Fortuna___pyx_scope_struct_1_genexpr {
@@ -1592,15 +1592,15 @@
   PyObject *__pyx_v_itm;
   PyObject *__pyx_t_0;
   Py_ssize_t __pyx_t_1;
   PyObject *(*__pyx_t_2)(PyObject *);
 };
 
 
-/* "Fortuna.pyx":874
+/* "Fortuna.pyx":889
  *             w_pair[0] = cum_weight
  *         self.max_weight = optimized_data[-1][0]
  *         self.data = tuple(tuple(itm) for itm in optimized_data)             # <<<<<<<<<<<<<<
  * 
  * 
  */
 struct __pyx_obj_7Fortuna___pyx_scope_struct_2_genexpr {
@@ -1609,15 +1609,15 @@
   PyObject *__pyx_v_itm;
   PyObject *__pyx_t_0;
   Py_ssize_t __pyx_t_1;
   PyObject *(*__pyx_t_2)(PyObject *);
 };
 
 
-/* "Fortuna.pyx":912
+/* "Fortuna.pyx":927
  *         self.choice_pack = (
  *             self.prompt,
  *             *(f"{k}. {v.title()}" for k, v in self.data.items()),             # <<<<<<<<<<<<<<
  *             self.cursor,
  *         )
  */
 struct __pyx_obj_7Fortuna___pyx_scope_struct_3_genexpr {
@@ -2755,15 +2755,15 @@
 static const char __pyx_k_itm[] = "itm";
 static const char __pyx_k_key[] = "key";
 static const char __pyx_k_low[] = "low";
 static const char __pyx_k_seq[] = "seq";
 static const char __pyx_k_str[] = "str";
 static const char __pyx_k_Dict[] = "Dict";
 static const char __pyx_k_None[] = "None";
-static const char __pyx_k__162[] = "?";
+static const char __pyx_k__165[] = "?";
 static const char __pyx_k_args[] = "args";
 static const char __pyx_k_beta[] = "beta";
 static const char __pyx_k_bool[] = "bool";
 static const char __pyx_k_call[] = "__call__";
 static const char __pyx_k_data[] = "data";
 static const char __pyx_k_dice[] = "dice";
 static const char __pyx_k_dict[] = "__dict__";
@@ -2790,20 +2790,22 @@
 static const char __pyx_k_5_5_1[] = "5.5.1";
 static const char __pyx_k_alpha[] = "alpha";
 static const char __pyx_k_array[] = "array";
 static const char __pyx_k_close[] = "close";
 static const char __pyx_k_cycle[] = "cycle";
 static const char __pyx_k_deque[] = "deque";
 static const char __pyx_k_float[] = "float";
+static const char __pyx_k_index[] = "index";
 static const char __pyx_k_input[] = "input";
 static const char __pyx_k_items[] = "items";
 static const char __pyx_k_kappa[] = "kappa";
 static const char __pyx_k_limit[] = "limit";
 static const char __pyx_k_lower[] = "lower";
 static const char __pyx_k_monty[] = "monty";
+static const char __pyx_k_pivot[] = "pivot";
 static const char __pyx_k_query[] = "query";
 static const char __pyx_k_range[] = "range";
 static const char __pyx_k_rolls[] = "rolls";
 static const char __pyx_k_scale[] = "scale";
 static const char __pyx_k_shape[] = "shape";
 static const char __pyx_k_sides[] = "sides";
 static const char __pyx_k_slots[] = "__slots__";
@@ -2847,14 +2849,15 @@
 static const char __pyx_k_prepare[] = "__prepare__";
 static const char __pyx_k_reverse[] = "reverse";
 static const char __pyx_k_shuffle[] = "shuffle";
 static const char __pyx_k_std_dev[] = "std_dev";
 static const char __pyx_k_version[] = "version";
 static const char __pyx_k_Callable[] = "Callable";
 static const char __pyx_k_Iterable[] = "Iterable";
+static const char __pyx_k_Iterator[] = "Iterator";
 static const char __pyx_k_ZeroCool[] = "ZeroCool";
 static const char __pyx_k_cat_keys[] = "cat_keys";
 static const char __pyx_k_dispatch[] = "dispatch";
 static const char __pyx_k_key_bias[] = "key_bias";
 static const char __pyx_k_location[] = "location";
 static const char __pyx_k_log_mean[] = "log_mean";
 static const char __pyx_k_max_uint[] = "max_uint";
@@ -2942,14 +2945,15 @@
 static const char __pyx_k_middle_poisson[] = "middle_poisson";
 static const char __pyx_k_normal_variate[] = "normal_variate";
 static const char __pyx_k_optimized_data[] = "optimized_data";
 static const char __pyx_k_pareto_variate[] = "pareto_variate";
 static const char __pyx_k_quantum_linear[] = "quantum_linear";
 static const char __pyx_k_ratio_of_truth[] = "ratio_of_truth";
 static const char __pyx_k_weighted_table[] = "weighted_table";
+static const char __pyx_k_TruffleShuffle2[] = "TruffleShuffle2";
 static const char __pyx_k_poisson_variate[] = "poisson_variate";
 static const char __pyx_k_quantum_poisson[] = "quantum_poisson";
 static const char __pyx_k_truffle_shuffle[] = "truffle_shuffle";
 static const char __pyx_k_weibull_variate[] = "weibull_variate";
 static const char __pyx_k_Callable_int_int[] = "Callable[[int], int]";
 static const char __pyx_k_binomial_variate[] = "binomial_variate";
 static const char __pyx_k_fisher_f_variate[] = "fisher_f_variate";
@@ -2980,14 +2984,16 @@
 static const char __pyx_k_plus_or_minus_linear[] = "plus_or_minus_linear";
 static const char __pyx_k_QuantumMonty_dispatch[] = "QuantumMonty.dispatch";
 static const char __pyx_k_TruffleShuffle___call[] = "TruffleShuffle.__call__";
 static const char __pyx_k_TruffleShuffle___init[] = "TruffleShuffle.__init__";
 static const char __pyx_k_WeightedChoice___call[] = "WeightedChoice.__call__";
 static const char __pyx_k_extreme_value_variate[] = "extreme_value_variate";
 static const char __pyx_k_RelativeWeightedChoice[] = "RelativeWeightedChoice";
+static const char __pyx_k_TruffleShuffle2___call[] = "TruffleShuffle2.__call__";
+static const char __pyx_k_TruffleShuffle2___init[] = "TruffleShuffle2.__init__";
 static const char __pyx_k_MultiChoice__get_answer[] = "MultiChoice._get_answer";
 static const char __pyx_k_QuantumMonty_back_gauss[] = "QuantumMonty.back_gauss";
 static const char __pyx_k_CumulativeWeightedChoice[] = "CumulativeWeightedChoice";
 static const char __pyx_k_DistributionRange___call[] = "DistributionRange.__call__";
 static const char __pyx_k_DistributionRange___init[] = "DistributionRange.__init__";
 static const char __pyx_k_QuantumMonty_back_linear[] = "QuantumMonty.back_linear";
 static const char __pyx_k_QuantumMonty_front_gauss[] = "QuantumMonty.front_gauss";
@@ -3003,15 +3009,15 @@
 static const char __pyx_k_QuantumMonty_quantum_gauss[] = "QuantumMonty.quantum_gauss";
 static const char __pyx_k_QuantumMonty_quantum_monty[] = "QuantumMonty.quantum_monty";
 static const char __pyx_k_cumulative_weighted_choice[] = "cumulative_weighted_choice";
 static const char __pyx_k_Input_Error_Empty_Container[] = "Input Error, Empty Container";
 static const char __pyx_k_QuantumMonty_middle_poisson[] = "QuantumMonty.middle_poisson";
 static const char __pyx_k_QuantumMonty_quantum_linear[] = "QuantumMonty.quantum_linear";
 static const char __pyx_k_QuantumMonty_quantum_poisson[] = "QuantumMonty.quantum_poisson";
-static const char __pyx_k_MultiChoice___init___line_881[] = "MultiChoice.__init__ (line 881)";
+static const char __pyx_k_MultiChoice___init___line_896[] = "MultiChoice.__init__ (line 896)";
 static const char __pyx_k_RelativeWeightedChoice___init[] = "RelativeWeightedChoice.__init__.<locals>.genexpr";
 static const char __pyx_k_truffle_shuffle_locals_worker[] = "truffle_shuffle.<locals>.worker";
 static const char __pyx_k_Flex_Cat_FlexCat_is_a_lot_like[] = " Flex Cat\n    FlexCat is a lot like a multidimensional QuantumMonty.\n\n    The initializer takes two optional keyword arguments to specify the\n    algorithms to be used to make random selections. The algorithm specified\n    for selecting a key need not be the same as the one for selecting values.\n    An optional key may be provided at call time to bypass the random\n    key selection. Keys passed in this way must exactly match a\n    key in the Matrix.\n\n    By default, FlexCat will use key_bias=\"front_linear\"\n    and val_bias=\"truffle_shuffle\", this will make the top of the data\n    structure geometrically more common than the bottom, and it will\n    truffle shuffle the sequence values. This config is known as TopCat,\n    it produces a descending-step, wide inner-distribution sequence.\n    Many other combinations are available.\n\n    Please refer to https://pypi.org/project/Fortuna/ for full documentation.\n    ";
 static const char __pyx_k_Quantum_Monty_param_collection[] = " Quantum Monty\n    @param collection : Collection of Values.\n    @param flat : Bool. Default is True. Option to automatically flatten\n        callable values with lazy evaluation.\n    @return : Callable Object with Monty Methods for producing various\n        distributions of the collection.\n        @param *args, **kwargs : Optional arguments used to flatten the return\n            Value (below) if Callable.\n        @return : Random value from the collection.\n\n    Please refer to https://pypi.org/project/Fortuna/ for full documentation.\n    ";
 static const char __pyx_k_CumulativeWeightedChoice___init[] = "CumulativeWeightedChoice.__init__.<locals>.genexpr";
 static const char __pyx_k_DistributionRange_param_zero_co[] = " DistributionRange\n\n    @param zero_cool: ZeroCool random distribution, F(N) -> [0, N-1]\n    @param lower: minimum\n    @param upper: maximum\n    ";
 static const char __pyx_k_Multiple_Choice_MultiChoice_gen[] = " Multiple Choice\n    MultiChoice: generates multiple choice style questions on the terminal. ";
@@ -3084,14 +3090,16 @@
 static PyObject *__pyx_pf_7Fortuna_90cumulative_weighted_choice(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_weighted_table); /* proto */
 static PyObject *__pyx_pf_7Fortuna_15truffle_shuffle_worker(PyObject *__pyx_self); /* proto */
 static PyObject *__pyx_pf_7Fortuna_92truffle_shuffle(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_data); /* proto */
 static PyObject *__pyx_pf_7Fortuna_94sample(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_population, PyObject *__pyx_v_k); /* proto */
 static PyObject *__pyx_pf_7Fortuna_148__defaults__(CYTHON_UNUSED PyObject *__pyx_self); /* proto */
 static PyObject *__pyx_pf_7Fortuna_11RandomValue___init__(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_collection, PyObject *__pyx_v_zero_cool, PyObject *__pyx_v_flat); /* proto */
 static PyObject *__pyx_pf_7Fortuna_11RandomValue_2__call__(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_args, PyObject *__pyx_v_kwargs); /* proto */
+static PyObject *__pyx_pf_7Fortuna_15TruffleShuffle2___init__(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_collection, PyObject *__pyx_v_flat); /* proto */
+static PyObject *__pyx_pf_7Fortuna_15TruffleShuffle2_2__call__(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_args, PyObject *__pyx_v_kwargs); /* proto */
 static PyObject *__pyx_pf_7Fortuna_14TruffleShuffle___init__(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_collection, PyObject *__pyx_v_flat); /* proto */
 static PyObject *__pyx_pf_7Fortuna_14TruffleShuffle_2__call__(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_args, PyObject *__pyx_v_kwargs); /* proto */
 static PyObject *__pyx_pf_7Fortuna_12QuantumMonty___init__(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_collection, PyObject *__pyx_v_flat); /* proto */
 static PyObject *__pyx_pf_7Fortuna_12QuantumMonty_2__call__(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_args, PyObject *__pyx_v_kwargs); /* proto */
 static PyObject *__pyx_pf_7Fortuna_12QuantumMonty_4dispatch(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_monty); /* proto */
 static PyObject *__pyx_pf_7Fortuna_12QuantumMonty_6flat_uniform(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_args, PyObject *__pyx_v_kwargs); /* proto */
 static PyObject *__pyx_pf_7Fortuna_12QuantumMonty_8cycle(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_args, PyObject *__pyx_v_kwargs); /* proto */
@@ -3202,18 +3210,19 @@
   PyObject *__pyx_n_s_FlexCat___init;
   PyObject *__pyx_kp_s_Flex_Cat_FlexCat_is_a_lot_like;
   PyObject *__pyx_n_s_Fortuna;
   PyObject *__pyx_kp_s_Fortuna_pyx;
   PyObject *__pyx_kp_u_Input_Error_Empty_Container;
   PyObject *__pyx_n_s_Iterable;
   PyObject *__pyx_kp_s_Iterable_str;
+  PyObject *__pyx_n_s_Iterator;
   PyObject *__pyx_n_s_MultiChoice;
   PyObject *__pyx_n_s_MultiChoice___call;
   PyObject *__pyx_n_s_MultiChoice___init;
-  PyObject *__pyx_kp_u_MultiChoice___init___line_881;
+  PyObject *__pyx_kp_u_MultiChoice___init___line_896;
   PyObject *__pyx_n_s_MultiChoice___init___locals_gene;
   PyObject *__pyx_n_s_MultiChoice__get_answer;
   PyObject *__pyx_kp_s_Multiple_Choice_MultiChoice_gen;
   PyObject *__pyx_kp_u_Multiple_Choice_param_query_Str;
   PyObject *__pyx_n_s_None;
   PyObject *__pyx_n_s_QuantumMonty;
   PyObject *__pyx_n_s_QuantumMonty___call;
@@ -3242,23 +3251,26 @@
   PyObject *__pyx_n_s_RelativeWeightedChoice;
   PyObject *__pyx_n_s_RelativeWeightedChoice___init;
   PyObject *__pyx_n_s_RelativeWeightedChoice___init_2;
   PyObject *__pyx_n_s_RelativeWeightedChoice___init_3;
   PyObject *__pyx_kp_s_Relative_Weighted_Choice;
   PyObject *__pyx_kp_u_Sample_size_k_is_larger_than_pop;
   PyObject *__pyx_n_s_TruffleShuffle;
+  PyObject *__pyx_n_s_TruffleShuffle2;
+  PyObject *__pyx_n_s_TruffleShuffle2___call;
+  PyObject *__pyx_n_s_TruffleShuffle2___init;
   PyObject *__pyx_n_s_TruffleShuffle___call;
   PyObject *__pyx_n_s_TruffleShuffle___init;
   PyObject *__pyx_kp_s_Truffle_Shuffle_Produces_random;
   PyObject *__pyx_n_s_TypeError;
   PyObject *__pyx_n_s_WeightedChoice;
   PyObject *__pyx_n_s_WeightedChoice___call;
   PyObject *__pyx_kp_s_Weighted_Choice_Base_Class_inte;
   PyObject *__pyx_n_s_ZeroCool;
-  PyObject *__pyx_n_s__162;
+  PyObject *__pyx_n_s__165;
   PyObject *__pyx_kp_u__2;
   PyObject *__pyx_kp_u__3;
   PyObject *__pyx_kp_u__4;
   PyObject *__pyx_kp_u__5;
   PyObject *__pyx_kp_u__6;
   PyObject *__pyx_kp_u__7;
   PyObject *__pyx_n_s_ability_dice;
@@ -3339,14 +3351,16 @@
   PyObject *__pyx_n_s_genexpr;
   PyObject *__pyx_n_s_geometric_variate;
   PyObject *__pyx_n_s_get_answer;
   PyObject *__pyx_n_s_hi;
   PyObject *__pyx_n_s_high;
   PyObject *__pyx_n_s_i;
   PyObject *__pyx_n_s_import;
+  PyObject *__pyx_n_s_index;
+  PyObject *__pyx_n_u_index;
   PyObject *__pyx_n_s_init;
   PyObject *__pyx_n_s_init_subclass;
   PyObject *__pyx_n_s_input;
   PyObject *__pyx_n_s_int;
   PyObject *__pyx_n_s_is_coroutine;
   PyObject *__pyx_kp_u_isenabled;
   PyObject *__pyx_n_s_items;
@@ -3404,14 +3418,16 @@
   PyObject *__pyx_n_s_normal_variate;
   PyObject *__pyx_n_s_number;
   PyObject *__pyx_n_s_number_of_trials;
   PyObject *__pyx_n_s_optimized_data;
   PyObject *__pyx_n_s_options;
   PyObject *__pyx_n_s_pareto_variate;
   PyObject *__pyx_n_s_percent_true;
+  PyObject *__pyx_n_s_pivot;
+  PyObject *__pyx_n_u_pivot;
   PyObject *__pyx_n_s_plus_or_minus;
   PyObject *__pyx_n_s_plus_or_minus_gauss;
   PyObject *__pyx_n_s_plus_or_minus_linear;
   PyObject *__pyx_n_s_poisson_variate;
   PyObject *__pyx_n_s_population;
   PyObject *__pyx_n_s_prepare;
   PyObject *__pyx_n_s_prev_weight;
@@ -3537,40 +3553,41 @@
   PyObject *__pyx_tuple__83;
   PyObject *__pyx_tuple__85;
   PyObject *__pyx_tuple__86;
   PyObject *__pyx_tuple__88;
   PyObject *__pyx_tuple__90;
   PyObject *__pyx_tuple__91;
   PyObject *__pyx_tuple__94;
+  PyObject *__pyx_tuple__97;
   PyObject *__pyx_codeobj__8;
-  PyObject *__pyx_tuple__111;
-  PyObject *__pyx_tuple__112;
   PyObject *__pyx_tuple__114;
   PyObject *__pyx_tuple__115;
   PyObject *__pyx_tuple__117;
   PyObject *__pyx_tuple__118;
-  PyObject *__pyx_tuple__119;
+  PyObject *__pyx_tuple__120;
   PyObject *__pyx_tuple__121;
-  PyObject *__pyx_tuple__123;
-  PyObject *__pyx_tuple__125;
+  PyObject *__pyx_tuple__122;
+  PyObject *__pyx_tuple__124;
+  PyObject *__pyx_tuple__126;
   PyObject *__pyx_tuple__128;
-  PyObject *__pyx_tuple__130;
-  PyObject *__pyx_tuple__132;
-  PyObject *__pyx_tuple__134;
-  PyObject *__pyx_tuple__136;
-  PyObject *__pyx_tuple__138;
+  PyObject *__pyx_tuple__131;
+  PyObject *__pyx_tuple__133;
+  PyObject *__pyx_tuple__135;
+  PyObject *__pyx_tuple__137;
+  PyObject *__pyx_tuple__139;
   PyObject *__pyx_tuple__141;
-  PyObject *__pyx_tuple__143;
-  PyObject *__pyx_tuple__145;
-  PyObject *__pyx_tuple__147;
+  PyObject *__pyx_tuple__144;
+  PyObject *__pyx_tuple__146;
+  PyObject *__pyx_tuple__148;
   PyObject *__pyx_tuple__150;
-  PyObject *__pyx_tuple__152;
-  PyObject *__pyx_tuple__154;
-  PyObject *__pyx_tuple__156;
+  PyObject *__pyx_tuple__153;
+  PyObject *__pyx_tuple__155;
+  PyObject *__pyx_tuple__157;
   PyObject *__pyx_tuple__159;
+  PyObject *__pyx_tuple__162;
   PyObject *__pyx_codeobj__10;
   PyObject *__pyx_codeobj__11;
   PyObject *__pyx_codeobj__12;
   PyObject *__pyx_codeobj__13;
   PyObject *__pyx_codeobj__14;
   PyObject *__pyx_codeobj__15;
   PyObject *__pyx_codeobj__16;
@@ -3620,54 +3637,56 @@
   PyObject *__pyx_codeobj__84;
   PyObject *__pyx_codeobj__87;
   PyObject *__pyx_codeobj__89;
   PyObject *__pyx_codeobj__92;
   PyObject *__pyx_codeobj__93;
   PyObject *__pyx_codeobj__95;
   PyObject *__pyx_codeobj__96;
-  PyObject *__pyx_codeobj__97;
   PyObject *__pyx_codeobj__98;
   PyObject *__pyx_codeobj__99;
   PyObject *__pyx_codeobj__100;
   PyObject *__pyx_codeobj__101;
   PyObject *__pyx_codeobj__102;
   PyObject *__pyx_codeobj__103;
   PyObject *__pyx_codeobj__104;
   PyObject *__pyx_codeobj__105;
   PyObject *__pyx_codeobj__106;
   PyObject *__pyx_codeobj__107;
   PyObject *__pyx_codeobj__108;
   PyObject *__pyx_codeobj__109;
   PyObject *__pyx_codeobj__110;
+  PyObject *__pyx_codeobj__111;
+  PyObject *__pyx_codeobj__112;
   PyObject *__pyx_codeobj__113;
   PyObject *__pyx_codeobj__116;
-  PyObject *__pyx_codeobj__120;
-  PyObject *__pyx_codeobj__122;
-  PyObject *__pyx_codeobj__124;
-  PyObject *__pyx_codeobj__126;
+  PyObject *__pyx_codeobj__119;
+  PyObject *__pyx_codeobj__123;
+  PyObject *__pyx_codeobj__125;
   PyObject *__pyx_codeobj__127;
   PyObject *__pyx_codeobj__129;
-  PyObject *__pyx_codeobj__131;
-  PyObject *__pyx_codeobj__133;
-  PyObject *__pyx_codeobj__135;
-  PyObject *__pyx_codeobj__137;
-  PyObject *__pyx_codeobj__139;
+  PyObject *__pyx_codeobj__130;
+  PyObject *__pyx_codeobj__132;
+  PyObject *__pyx_codeobj__134;
+  PyObject *__pyx_codeobj__136;
+  PyObject *__pyx_codeobj__138;
   PyObject *__pyx_codeobj__140;
   PyObject *__pyx_codeobj__142;
-  PyObject *__pyx_codeobj__144;
-  PyObject *__pyx_codeobj__146;
-  PyObject *__pyx_codeobj__148;
+  PyObject *__pyx_codeobj__143;
+  PyObject *__pyx_codeobj__145;
+  PyObject *__pyx_codeobj__147;
   PyObject *__pyx_codeobj__149;
   PyObject *__pyx_codeobj__151;
-  PyObject *__pyx_codeobj__153;
-  PyObject *__pyx_codeobj__155;
-  PyObject *__pyx_codeobj__157;
+  PyObject *__pyx_codeobj__152;
+  PyObject *__pyx_codeobj__154;
+  PyObject *__pyx_codeobj__156;
   PyObject *__pyx_codeobj__158;
   PyObject *__pyx_codeobj__160;
   PyObject *__pyx_codeobj__161;
+  PyObject *__pyx_codeobj__163;
+  PyObject *__pyx_codeobj__164;
 } __pyx_mstate;
 
 #if CYTHON_USE_MODULE_STATE
 #ifdef __cplusplus
 namespace {
   extern struct PyModuleDef __pyx_moduledef;
 } /* anonymous namespace */
@@ -3733,18 +3752,19 @@
   Py_CLEAR(clear_module_state->__pyx_n_s_FlexCat___init);
   Py_CLEAR(clear_module_state->__pyx_kp_s_Flex_Cat_FlexCat_is_a_lot_like);
   Py_CLEAR(clear_module_state->__pyx_n_s_Fortuna);
   Py_CLEAR(clear_module_state->__pyx_kp_s_Fortuna_pyx);
   Py_CLEAR(clear_module_state->__pyx_kp_u_Input_Error_Empty_Container);
   Py_CLEAR(clear_module_state->__pyx_n_s_Iterable);
   Py_CLEAR(clear_module_state->__pyx_kp_s_Iterable_str);
+  Py_CLEAR(clear_module_state->__pyx_n_s_Iterator);
   Py_CLEAR(clear_module_state->__pyx_n_s_MultiChoice);
   Py_CLEAR(clear_module_state->__pyx_n_s_MultiChoice___call);
   Py_CLEAR(clear_module_state->__pyx_n_s_MultiChoice___init);
-  Py_CLEAR(clear_module_state->__pyx_kp_u_MultiChoice___init___line_881);
+  Py_CLEAR(clear_module_state->__pyx_kp_u_MultiChoice___init___line_896);
   Py_CLEAR(clear_module_state->__pyx_n_s_MultiChoice___init___locals_gene);
   Py_CLEAR(clear_module_state->__pyx_n_s_MultiChoice__get_answer);
   Py_CLEAR(clear_module_state->__pyx_kp_s_Multiple_Choice_MultiChoice_gen);
   Py_CLEAR(clear_module_state->__pyx_kp_u_Multiple_Choice_param_query_Str);
   Py_CLEAR(clear_module_state->__pyx_n_s_None);
   Py_CLEAR(clear_module_state->__pyx_n_s_QuantumMonty);
   Py_CLEAR(clear_module_state->__pyx_n_s_QuantumMonty___call);
@@ -3773,23 +3793,26 @@
   Py_CLEAR(clear_module_state->__pyx_n_s_RelativeWeightedChoice);
   Py_CLEAR(clear_module_state->__pyx_n_s_RelativeWeightedChoice___init);
   Py_CLEAR(clear_module_state->__pyx_n_s_RelativeWeightedChoice___init_2);
   Py_CLEAR(clear_module_state->__pyx_n_s_RelativeWeightedChoice___init_3);
   Py_CLEAR(clear_module_state->__pyx_kp_s_Relative_Weighted_Choice);
   Py_CLEAR(clear_module_state->__pyx_kp_u_Sample_size_k_is_larger_than_pop);
   Py_CLEAR(clear_module_state->__pyx_n_s_TruffleShuffle);
+  Py_CLEAR(clear_module_state->__pyx_n_s_TruffleShuffle2);
+  Py_CLEAR(clear_module_state->__pyx_n_s_TruffleShuffle2___call);
+  Py_CLEAR(clear_module_state->__pyx_n_s_TruffleShuffle2___init);
   Py_CLEAR(clear_module_state->__pyx_n_s_TruffleShuffle___call);
   Py_CLEAR(clear_module_state->__pyx_n_s_TruffleShuffle___init);
   Py_CLEAR(clear_module_state->__pyx_kp_s_Truffle_Shuffle_Produces_random);
   Py_CLEAR(clear_module_state->__pyx_n_s_TypeError);
   Py_CLEAR(clear_module_state->__pyx_n_s_WeightedChoice);
   Py_CLEAR(clear_module_state->__pyx_n_s_WeightedChoice___call);
   Py_CLEAR(clear_module_state->__pyx_kp_s_Weighted_Choice_Base_Class_inte);
   Py_CLEAR(clear_module_state->__pyx_n_s_ZeroCool);
-  Py_CLEAR(clear_module_state->__pyx_n_s__162);
+  Py_CLEAR(clear_module_state->__pyx_n_s__165);
   Py_CLEAR(clear_module_state->__pyx_kp_u__2);
   Py_CLEAR(clear_module_state->__pyx_kp_u__3);
   Py_CLEAR(clear_module_state->__pyx_kp_u__4);
   Py_CLEAR(clear_module_state->__pyx_kp_u__5);
   Py_CLEAR(clear_module_state->__pyx_kp_u__6);
   Py_CLEAR(clear_module_state->__pyx_kp_u__7);
   Py_CLEAR(clear_module_state->__pyx_n_s_ability_dice);
@@ -3870,14 +3893,16 @@
   Py_CLEAR(clear_module_state->__pyx_n_s_genexpr);
   Py_CLEAR(clear_module_state->__pyx_n_s_geometric_variate);
   Py_CLEAR(clear_module_state->__pyx_n_s_get_answer);
   Py_CLEAR(clear_module_state->__pyx_n_s_hi);
   Py_CLEAR(clear_module_state->__pyx_n_s_high);
   Py_CLEAR(clear_module_state->__pyx_n_s_i);
   Py_CLEAR(clear_module_state->__pyx_n_s_import);
+  Py_CLEAR(clear_module_state->__pyx_n_s_index);
+  Py_CLEAR(clear_module_state->__pyx_n_u_index);
   Py_CLEAR(clear_module_state->__pyx_n_s_init);
   Py_CLEAR(clear_module_state->__pyx_n_s_init_subclass);
   Py_CLEAR(clear_module_state->__pyx_n_s_input);
   Py_CLEAR(clear_module_state->__pyx_n_s_int);
   Py_CLEAR(clear_module_state->__pyx_n_s_is_coroutine);
   Py_CLEAR(clear_module_state->__pyx_kp_u_isenabled);
   Py_CLEAR(clear_module_state->__pyx_n_s_items);
@@ -3935,14 +3960,16 @@
   Py_CLEAR(clear_module_state->__pyx_n_s_normal_variate);
   Py_CLEAR(clear_module_state->__pyx_n_s_number);
   Py_CLEAR(clear_module_state->__pyx_n_s_number_of_trials);
   Py_CLEAR(clear_module_state->__pyx_n_s_optimized_data);
   Py_CLEAR(clear_module_state->__pyx_n_s_options);
   Py_CLEAR(clear_module_state->__pyx_n_s_pareto_variate);
   Py_CLEAR(clear_module_state->__pyx_n_s_percent_true);
+  Py_CLEAR(clear_module_state->__pyx_n_s_pivot);
+  Py_CLEAR(clear_module_state->__pyx_n_u_pivot);
   Py_CLEAR(clear_module_state->__pyx_n_s_plus_or_minus);
   Py_CLEAR(clear_module_state->__pyx_n_s_plus_or_minus_gauss);
   Py_CLEAR(clear_module_state->__pyx_n_s_plus_or_minus_linear);
   Py_CLEAR(clear_module_state->__pyx_n_s_poisson_variate);
   Py_CLEAR(clear_module_state->__pyx_n_s_population);
   Py_CLEAR(clear_module_state->__pyx_n_s_prepare);
   Py_CLEAR(clear_module_state->__pyx_n_s_prev_weight);
@@ -4068,40 +4095,41 @@
   Py_CLEAR(clear_module_state->__pyx_tuple__83);
   Py_CLEAR(clear_module_state->__pyx_tuple__85);
   Py_CLEAR(clear_module_state->__pyx_tuple__86);
   Py_CLEAR(clear_module_state->__pyx_tuple__88);
   Py_CLEAR(clear_module_state->__pyx_tuple__90);
   Py_CLEAR(clear_module_state->__pyx_tuple__91);
   Py_CLEAR(clear_module_state->__pyx_tuple__94);
+  Py_CLEAR(clear_module_state->__pyx_tuple__97);
   Py_CLEAR(clear_module_state->__pyx_codeobj__8);
-  Py_CLEAR(clear_module_state->__pyx_tuple__111);
-  Py_CLEAR(clear_module_state->__pyx_tuple__112);
   Py_CLEAR(clear_module_state->__pyx_tuple__114);
   Py_CLEAR(clear_module_state->__pyx_tuple__115);
   Py_CLEAR(clear_module_state->__pyx_tuple__117);
   Py_CLEAR(clear_module_state->__pyx_tuple__118);
-  Py_CLEAR(clear_module_state->__pyx_tuple__119);
+  Py_CLEAR(clear_module_state->__pyx_tuple__120);
   Py_CLEAR(clear_module_state->__pyx_tuple__121);
-  Py_CLEAR(clear_module_state->__pyx_tuple__123);
-  Py_CLEAR(clear_module_state->__pyx_tuple__125);
+  Py_CLEAR(clear_module_state->__pyx_tuple__122);
+  Py_CLEAR(clear_module_state->__pyx_tuple__124);
+  Py_CLEAR(clear_module_state->__pyx_tuple__126);
   Py_CLEAR(clear_module_state->__pyx_tuple__128);
-  Py_CLEAR(clear_module_state->__pyx_tuple__130);
-  Py_CLEAR(clear_module_state->__pyx_tuple__132);
-  Py_CLEAR(clear_module_state->__pyx_tuple__134);
-  Py_CLEAR(clear_module_state->__pyx_tuple__136);
-  Py_CLEAR(clear_module_state->__pyx_tuple__138);
+  Py_CLEAR(clear_module_state->__pyx_tuple__131);
+  Py_CLEAR(clear_module_state->__pyx_tuple__133);
+  Py_CLEAR(clear_module_state->__pyx_tuple__135);
+  Py_CLEAR(clear_module_state->__pyx_tuple__137);
+  Py_CLEAR(clear_module_state->__pyx_tuple__139);
   Py_CLEAR(clear_module_state->__pyx_tuple__141);
-  Py_CLEAR(clear_module_state->__pyx_tuple__143);
-  Py_CLEAR(clear_module_state->__pyx_tuple__145);
-  Py_CLEAR(clear_module_state->__pyx_tuple__147);
+  Py_CLEAR(clear_module_state->__pyx_tuple__144);
+  Py_CLEAR(clear_module_state->__pyx_tuple__146);
+  Py_CLEAR(clear_module_state->__pyx_tuple__148);
   Py_CLEAR(clear_module_state->__pyx_tuple__150);
-  Py_CLEAR(clear_module_state->__pyx_tuple__152);
-  Py_CLEAR(clear_module_state->__pyx_tuple__154);
-  Py_CLEAR(clear_module_state->__pyx_tuple__156);
+  Py_CLEAR(clear_module_state->__pyx_tuple__153);
+  Py_CLEAR(clear_module_state->__pyx_tuple__155);
+  Py_CLEAR(clear_module_state->__pyx_tuple__157);
   Py_CLEAR(clear_module_state->__pyx_tuple__159);
+  Py_CLEAR(clear_module_state->__pyx_tuple__162);
   Py_CLEAR(clear_module_state->__pyx_codeobj__10);
   Py_CLEAR(clear_module_state->__pyx_codeobj__11);
   Py_CLEAR(clear_module_state->__pyx_codeobj__12);
   Py_CLEAR(clear_module_state->__pyx_codeobj__13);
   Py_CLEAR(clear_module_state->__pyx_codeobj__14);
   Py_CLEAR(clear_module_state->__pyx_codeobj__15);
   Py_CLEAR(clear_module_state->__pyx_codeobj__16);
@@ -4151,54 +4179,56 @@
   Py_CLEAR(clear_module_state->__pyx_codeobj__84);
   Py_CLEAR(clear_module_state->__pyx_codeobj__87);
   Py_CLEAR(clear_module_state->__pyx_codeobj__89);
   Py_CLEAR(clear_module_state->__pyx_codeobj__92);
   Py_CLEAR(clear_module_state->__pyx_codeobj__93);
   Py_CLEAR(clear_module_state->__pyx_codeobj__95);
   Py_CLEAR(clear_module_state->__pyx_codeobj__96);
-  Py_CLEAR(clear_module_state->__pyx_codeobj__97);
   Py_CLEAR(clear_module_state->__pyx_codeobj__98);
   Py_CLEAR(clear_module_state->__pyx_codeobj__99);
   Py_CLEAR(clear_module_state->__pyx_codeobj__100);
   Py_CLEAR(clear_module_state->__pyx_codeobj__101);
   Py_CLEAR(clear_module_state->__pyx_codeobj__102);
   Py_CLEAR(clear_module_state->__pyx_codeobj__103);
   Py_CLEAR(clear_module_state->__pyx_codeobj__104);
   Py_CLEAR(clear_module_state->__pyx_codeobj__105);
   Py_CLEAR(clear_module_state->__pyx_codeobj__106);
   Py_CLEAR(clear_module_state->__pyx_codeobj__107);
   Py_CLEAR(clear_module_state->__pyx_codeobj__108);
   Py_CLEAR(clear_module_state->__pyx_codeobj__109);
   Py_CLEAR(clear_module_state->__pyx_codeobj__110);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__111);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__112);
   Py_CLEAR(clear_module_state->__pyx_codeobj__113);
   Py_CLEAR(clear_module_state->__pyx_codeobj__116);
-  Py_CLEAR(clear_module_state->__pyx_codeobj__120);
-  Py_CLEAR(clear_module_state->__pyx_codeobj__122);
-  Py_CLEAR(clear_module_state->__pyx_codeobj__124);
-  Py_CLEAR(clear_module_state->__pyx_codeobj__126);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__119);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__123);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__125);
   Py_CLEAR(clear_module_state->__pyx_codeobj__127);
   Py_CLEAR(clear_module_state->__pyx_codeobj__129);
-  Py_CLEAR(clear_module_state->__pyx_codeobj__131);
-  Py_CLEAR(clear_module_state->__pyx_codeobj__133);
-  Py_CLEAR(clear_module_state->__pyx_codeobj__135);
-  Py_CLEAR(clear_module_state->__pyx_codeobj__137);
-  Py_CLEAR(clear_module_state->__pyx_codeobj__139);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__130);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__132);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__134);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__136);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__138);
   Py_CLEAR(clear_module_state->__pyx_codeobj__140);
   Py_CLEAR(clear_module_state->__pyx_codeobj__142);
-  Py_CLEAR(clear_module_state->__pyx_codeobj__144);
-  Py_CLEAR(clear_module_state->__pyx_codeobj__146);
-  Py_CLEAR(clear_module_state->__pyx_codeobj__148);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__143);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__145);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__147);
   Py_CLEAR(clear_module_state->__pyx_codeobj__149);
   Py_CLEAR(clear_module_state->__pyx_codeobj__151);
-  Py_CLEAR(clear_module_state->__pyx_codeobj__153);
-  Py_CLEAR(clear_module_state->__pyx_codeobj__155);
-  Py_CLEAR(clear_module_state->__pyx_codeobj__157);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__152);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__154);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__156);
   Py_CLEAR(clear_module_state->__pyx_codeobj__158);
   Py_CLEAR(clear_module_state->__pyx_codeobj__160);
   Py_CLEAR(clear_module_state->__pyx_codeobj__161);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__163);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__164);
   return 0;
 }
 #endif
 /* #### Code section: module_state_traverse ### */
 #if CYTHON_USE_MODULE_STATE
 static int __pyx_m_traverse(PyObject *m, visitproc visit, void *arg) {
   __pyx_mstate *traverse_module_state = __pyx_mstate(m);
@@ -4242,18 +4272,19 @@
   Py_VISIT(traverse_module_state->__pyx_n_s_FlexCat___init);
   Py_VISIT(traverse_module_state->__pyx_kp_s_Flex_Cat_FlexCat_is_a_lot_like);
   Py_VISIT(traverse_module_state->__pyx_n_s_Fortuna);
   Py_VISIT(traverse_module_state->__pyx_kp_s_Fortuna_pyx);
   Py_VISIT(traverse_module_state->__pyx_kp_u_Input_Error_Empty_Container);
   Py_VISIT(traverse_module_state->__pyx_n_s_Iterable);
   Py_VISIT(traverse_module_state->__pyx_kp_s_Iterable_str);
+  Py_VISIT(traverse_module_state->__pyx_n_s_Iterator);
   Py_VISIT(traverse_module_state->__pyx_n_s_MultiChoice);
   Py_VISIT(traverse_module_state->__pyx_n_s_MultiChoice___call);
   Py_VISIT(traverse_module_state->__pyx_n_s_MultiChoice___init);
-  Py_VISIT(traverse_module_state->__pyx_kp_u_MultiChoice___init___line_881);
+  Py_VISIT(traverse_module_state->__pyx_kp_u_MultiChoice___init___line_896);
   Py_VISIT(traverse_module_state->__pyx_n_s_MultiChoice___init___locals_gene);
   Py_VISIT(traverse_module_state->__pyx_n_s_MultiChoice__get_answer);
   Py_VISIT(traverse_module_state->__pyx_kp_s_Multiple_Choice_MultiChoice_gen);
   Py_VISIT(traverse_module_state->__pyx_kp_u_Multiple_Choice_param_query_Str);
   Py_VISIT(traverse_module_state->__pyx_n_s_None);
   Py_VISIT(traverse_module_state->__pyx_n_s_QuantumMonty);
   Py_VISIT(traverse_module_state->__pyx_n_s_QuantumMonty___call);
@@ -4282,23 +4313,26 @@
   Py_VISIT(traverse_module_state->__pyx_n_s_RelativeWeightedChoice);
   Py_VISIT(traverse_module_state->__pyx_n_s_RelativeWeightedChoice___init);
   Py_VISIT(traverse_module_state->__pyx_n_s_RelativeWeightedChoice___init_2);
   Py_VISIT(traverse_module_state->__pyx_n_s_RelativeWeightedChoice___init_3);
   Py_VISIT(traverse_module_state->__pyx_kp_s_Relative_Weighted_Choice);
   Py_VISIT(traverse_module_state->__pyx_kp_u_Sample_size_k_is_larger_than_pop);
   Py_VISIT(traverse_module_state->__pyx_n_s_TruffleShuffle);
+  Py_VISIT(traverse_module_state->__pyx_n_s_TruffleShuffle2);
+  Py_VISIT(traverse_module_state->__pyx_n_s_TruffleShuffle2___call);
+  Py_VISIT(traverse_module_state->__pyx_n_s_TruffleShuffle2___init);
   Py_VISIT(traverse_module_state->__pyx_n_s_TruffleShuffle___call);
   Py_VISIT(traverse_module_state->__pyx_n_s_TruffleShuffle___init);
   Py_VISIT(traverse_module_state->__pyx_kp_s_Truffle_Shuffle_Produces_random);
   Py_VISIT(traverse_module_state->__pyx_n_s_TypeError);
   Py_VISIT(traverse_module_state->__pyx_n_s_WeightedChoice);
   Py_VISIT(traverse_module_state->__pyx_n_s_WeightedChoice___call);
   Py_VISIT(traverse_module_state->__pyx_kp_s_Weighted_Choice_Base_Class_inte);
   Py_VISIT(traverse_module_state->__pyx_n_s_ZeroCool);
-  Py_VISIT(traverse_module_state->__pyx_n_s__162);
+  Py_VISIT(traverse_module_state->__pyx_n_s__165);
   Py_VISIT(traverse_module_state->__pyx_kp_u__2);
   Py_VISIT(traverse_module_state->__pyx_kp_u__3);
   Py_VISIT(traverse_module_state->__pyx_kp_u__4);
   Py_VISIT(traverse_module_state->__pyx_kp_u__5);
   Py_VISIT(traverse_module_state->__pyx_kp_u__6);
   Py_VISIT(traverse_module_state->__pyx_kp_u__7);
   Py_VISIT(traverse_module_state->__pyx_n_s_ability_dice);
@@ -4379,14 +4413,16 @@
   Py_VISIT(traverse_module_state->__pyx_n_s_genexpr);
   Py_VISIT(traverse_module_state->__pyx_n_s_geometric_variate);
   Py_VISIT(traverse_module_state->__pyx_n_s_get_answer);
   Py_VISIT(traverse_module_state->__pyx_n_s_hi);
   Py_VISIT(traverse_module_state->__pyx_n_s_high);
   Py_VISIT(traverse_module_state->__pyx_n_s_i);
   Py_VISIT(traverse_module_state->__pyx_n_s_import);
+  Py_VISIT(traverse_module_state->__pyx_n_s_index);
+  Py_VISIT(traverse_module_state->__pyx_n_u_index);
   Py_VISIT(traverse_module_state->__pyx_n_s_init);
   Py_VISIT(traverse_module_state->__pyx_n_s_init_subclass);
   Py_VISIT(traverse_module_state->__pyx_n_s_input);
   Py_VISIT(traverse_module_state->__pyx_n_s_int);
   Py_VISIT(traverse_module_state->__pyx_n_s_is_coroutine);
   Py_VISIT(traverse_module_state->__pyx_kp_u_isenabled);
   Py_VISIT(traverse_module_state->__pyx_n_s_items);
@@ -4444,14 +4480,16 @@
   Py_VISIT(traverse_module_state->__pyx_n_s_normal_variate);
   Py_VISIT(traverse_module_state->__pyx_n_s_number);
   Py_VISIT(traverse_module_state->__pyx_n_s_number_of_trials);
   Py_VISIT(traverse_module_state->__pyx_n_s_optimized_data);
   Py_VISIT(traverse_module_state->__pyx_n_s_options);
   Py_VISIT(traverse_module_state->__pyx_n_s_pareto_variate);
   Py_VISIT(traverse_module_state->__pyx_n_s_percent_true);
+  Py_VISIT(traverse_module_state->__pyx_n_s_pivot);
+  Py_VISIT(traverse_module_state->__pyx_n_u_pivot);
   Py_VISIT(traverse_module_state->__pyx_n_s_plus_or_minus);
   Py_VISIT(traverse_module_state->__pyx_n_s_plus_or_minus_gauss);
   Py_VISIT(traverse_module_state->__pyx_n_s_plus_or_minus_linear);
   Py_VISIT(traverse_module_state->__pyx_n_s_poisson_variate);
   Py_VISIT(traverse_module_state->__pyx_n_s_population);
   Py_VISIT(traverse_module_state->__pyx_n_s_prepare);
   Py_VISIT(traverse_module_state->__pyx_n_s_prev_weight);
@@ -4577,40 +4615,41 @@
   Py_VISIT(traverse_module_state->__pyx_tuple__83);
   Py_VISIT(traverse_module_state->__pyx_tuple__85);
   Py_VISIT(traverse_module_state->__pyx_tuple__86);
   Py_VISIT(traverse_module_state->__pyx_tuple__88);
   Py_VISIT(traverse_module_state->__pyx_tuple__90);
   Py_VISIT(traverse_module_state->__pyx_tuple__91);
   Py_VISIT(traverse_module_state->__pyx_tuple__94);
+  Py_VISIT(traverse_module_state->__pyx_tuple__97);
   Py_VISIT(traverse_module_state->__pyx_codeobj__8);
-  Py_VISIT(traverse_module_state->__pyx_tuple__111);
-  Py_VISIT(traverse_module_state->__pyx_tuple__112);
   Py_VISIT(traverse_module_state->__pyx_tuple__114);
   Py_VISIT(traverse_module_state->__pyx_tuple__115);
   Py_VISIT(traverse_module_state->__pyx_tuple__117);
   Py_VISIT(traverse_module_state->__pyx_tuple__118);
-  Py_VISIT(traverse_module_state->__pyx_tuple__119);
+  Py_VISIT(traverse_module_state->__pyx_tuple__120);
   Py_VISIT(traverse_module_state->__pyx_tuple__121);
-  Py_VISIT(traverse_module_state->__pyx_tuple__123);
-  Py_VISIT(traverse_module_state->__pyx_tuple__125);
+  Py_VISIT(traverse_module_state->__pyx_tuple__122);
+  Py_VISIT(traverse_module_state->__pyx_tuple__124);
+  Py_VISIT(traverse_module_state->__pyx_tuple__126);
   Py_VISIT(traverse_module_state->__pyx_tuple__128);
-  Py_VISIT(traverse_module_state->__pyx_tuple__130);
-  Py_VISIT(traverse_module_state->__pyx_tuple__132);
-  Py_VISIT(traverse_module_state->__pyx_tuple__134);
-  Py_VISIT(traverse_module_state->__pyx_tuple__136);
-  Py_VISIT(traverse_module_state->__pyx_tuple__138);
+  Py_VISIT(traverse_module_state->__pyx_tuple__131);
+  Py_VISIT(traverse_module_state->__pyx_tuple__133);
+  Py_VISIT(traverse_module_state->__pyx_tuple__135);
+  Py_VISIT(traverse_module_state->__pyx_tuple__137);
+  Py_VISIT(traverse_module_state->__pyx_tuple__139);
   Py_VISIT(traverse_module_state->__pyx_tuple__141);
-  Py_VISIT(traverse_module_state->__pyx_tuple__143);
-  Py_VISIT(traverse_module_state->__pyx_tuple__145);
-  Py_VISIT(traverse_module_state->__pyx_tuple__147);
+  Py_VISIT(traverse_module_state->__pyx_tuple__144);
+  Py_VISIT(traverse_module_state->__pyx_tuple__146);
+  Py_VISIT(traverse_module_state->__pyx_tuple__148);
   Py_VISIT(traverse_module_state->__pyx_tuple__150);
-  Py_VISIT(traverse_module_state->__pyx_tuple__152);
-  Py_VISIT(traverse_module_state->__pyx_tuple__154);
-  Py_VISIT(traverse_module_state->__pyx_tuple__156);
+  Py_VISIT(traverse_module_state->__pyx_tuple__153);
+  Py_VISIT(traverse_module_state->__pyx_tuple__155);
+  Py_VISIT(traverse_module_state->__pyx_tuple__157);
   Py_VISIT(traverse_module_state->__pyx_tuple__159);
+  Py_VISIT(traverse_module_state->__pyx_tuple__162);
   Py_VISIT(traverse_module_state->__pyx_codeobj__10);
   Py_VISIT(traverse_module_state->__pyx_codeobj__11);
   Py_VISIT(traverse_module_state->__pyx_codeobj__12);
   Py_VISIT(traverse_module_state->__pyx_codeobj__13);
   Py_VISIT(traverse_module_state->__pyx_codeobj__14);
   Py_VISIT(traverse_module_state->__pyx_codeobj__15);
   Py_VISIT(traverse_module_state->__pyx_codeobj__16);
@@ -4660,54 +4699,56 @@
   Py_VISIT(traverse_module_state->__pyx_codeobj__84);
   Py_VISIT(traverse_module_state->__pyx_codeobj__87);
   Py_VISIT(traverse_module_state->__pyx_codeobj__89);
   Py_VISIT(traverse_module_state->__pyx_codeobj__92);
   Py_VISIT(traverse_module_state->__pyx_codeobj__93);
   Py_VISIT(traverse_module_state->__pyx_codeobj__95);
   Py_VISIT(traverse_module_state->__pyx_codeobj__96);
-  Py_VISIT(traverse_module_state->__pyx_codeobj__97);
   Py_VISIT(traverse_module_state->__pyx_codeobj__98);
   Py_VISIT(traverse_module_state->__pyx_codeobj__99);
   Py_VISIT(traverse_module_state->__pyx_codeobj__100);
   Py_VISIT(traverse_module_state->__pyx_codeobj__101);
   Py_VISIT(traverse_module_state->__pyx_codeobj__102);
   Py_VISIT(traverse_module_state->__pyx_codeobj__103);
   Py_VISIT(traverse_module_state->__pyx_codeobj__104);
   Py_VISIT(traverse_module_state->__pyx_codeobj__105);
   Py_VISIT(traverse_module_state->__pyx_codeobj__106);
   Py_VISIT(traverse_module_state->__pyx_codeobj__107);
   Py_VISIT(traverse_module_state->__pyx_codeobj__108);
   Py_VISIT(traverse_module_state->__pyx_codeobj__109);
   Py_VISIT(traverse_module_state->__pyx_codeobj__110);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__111);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__112);
   Py_VISIT(traverse_module_state->__pyx_codeobj__113);
   Py_VISIT(traverse_module_state->__pyx_codeobj__116);
-  Py_VISIT(traverse_module_state->__pyx_codeobj__120);
-  Py_VISIT(traverse_module_state->__pyx_codeobj__122);
-  Py_VISIT(traverse_module_state->__pyx_codeobj__124);
-  Py_VISIT(traverse_module_state->__pyx_codeobj__126);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__119);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__123);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__125);
   Py_VISIT(traverse_module_state->__pyx_codeobj__127);
   Py_VISIT(traverse_module_state->__pyx_codeobj__129);
-  Py_VISIT(traverse_module_state->__pyx_codeobj__131);
-  Py_VISIT(traverse_module_state->__pyx_codeobj__133);
-  Py_VISIT(traverse_module_state->__pyx_codeobj__135);
-  Py_VISIT(traverse_module_state->__pyx_codeobj__137);
-  Py_VISIT(traverse_module_state->__pyx_codeobj__139);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__130);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__132);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__134);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__136);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__138);
   Py_VISIT(traverse_module_state->__pyx_codeobj__140);
   Py_VISIT(traverse_module_state->__pyx_codeobj__142);
-  Py_VISIT(traverse_module_state->__pyx_codeobj__144);
-  Py_VISIT(traverse_module_state->__pyx_codeobj__146);
-  Py_VISIT(traverse_module_state->__pyx_codeobj__148);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__143);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__145);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__147);
   Py_VISIT(traverse_module_state->__pyx_codeobj__149);
   Py_VISIT(traverse_module_state->__pyx_codeobj__151);
-  Py_VISIT(traverse_module_state->__pyx_codeobj__153);
-  Py_VISIT(traverse_module_state->__pyx_codeobj__155);
-  Py_VISIT(traverse_module_state->__pyx_codeobj__157);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__152);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__154);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__156);
   Py_VISIT(traverse_module_state->__pyx_codeobj__158);
   Py_VISIT(traverse_module_state->__pyx_codeobj__160);
   Py_VISIT(traverse_module_state->__pyx_codeobj__161);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__163);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__164);
   return 0;
 }
 #endif
 /* #### Code section: module_state_defines ### */
 #define __pyx_d __pyx_mstate_global->__pyx_d
 #define __pyx_b __pyx_mstate_global->__pyx_b
 #define __pyx_cython_runtime __pyx_mstate_global->__pyx_cython_runtime
@@ -4761,18 +4802,19 @@
 #define __pyx_n_s_FlexCat___init __pyx_mstate_global->__pyx_n_s_FlexCat___init
 #define __pyx_kp_s_Flex_Cat_FlexCat_is_a_lot_like __pyx_mstate_global->__pyx_kp_s_Flex_Cat_FlexCat_is_a_lot_like
 #define __pyx_n_s_Fortuna __pyx_mstate_global->__pyx_n_s_Fortuna
 #define __pyx_kp_s_Fortuna_pyx __pyx_mstate_global->__pyx_kp_s_Fortuna_pyx
 #define __pyx_kp_u_Input_Error_Empty_Container __pyx_mstate_global->__pyx_kp_u_Input_Error_Empty_Container
 #define __pyx_n_s_Iterable __pyx_mstate_global->__pyx_n_s_Iterable
 #define __pyx_kp_s_Iterable_str __pyx_mstate_global->__pyx_kp_s_Iterable_str
+#define __pyx_n_s_Iterator __pyx_mstate_global->__pyx_n_s_Iterator
 #define __pyx_n_s_MultiChoice __pyx_mstate_global->__pyx_n_s_MultiChoice
 #define __pyx_n_s_MultiChoice___call __pyx_mstate_global->__pyx_n_s_MultiChoice___call
 #define __pyx_n_s_MultiChoice___init __pyx_mstate_global->__pyx_n_s_MultiChoice___init
-#define __pyx_kp_u_MultiChoice___init___line_881 __pyx_mstate_global->__pyx_kp_u_MultiChoice___init___line_881
+#define __pyx_kp_u_MultiChoice___init___line_896 __pyx_mstate_global->__pyx_kp_u_MultiChoice___init___line_896
 #define __pyx_n_s_MultiChoice___init___locals_gene __pyx_mstate_global->__pyx_n_s_MultiChoice___init___locals_gene
 #define __pyx_n_s_MultiChoice__get_answer __pyx_mstate_global->__pyx_n_s_MultiChoice__get_answer
 #define __pyx_kp_s_Multiple_Choice_MultiChoice_gen __pyx_mstate_global->__pyx_kp_s_Multiple_Choice_MultiChoice_gen
 #define __pyx_kp_u_Multiple_Choice_param_query_Str __pyx_mstate_global->__pyx_kp_u_Multiple_Choice_param_query_Str
 #define __pyx_n_s_None __pyx_mstate_global->__pyx_n_s_None
 #define __pyx_n_s_QuantumMonty __pyx_mstate_global->__pyx_n_s_QuantumMonty
 #define __pyx_n_s_QuantumMonty___call __pyx_mstate_global->__pyx_n_s_QuantumMonty___call
@@ -4801,23 +4843,26 @@
 #define __pyx_n_s_RelativeWeightedChoice __pyx_mstate_global->__pyx_n_s_RelativeWeightedChoice
 #define __pyx_n_s_RelativeWeightedChoice___init __pyx_mstate_global->__pyx_n_s_RelativeWeightedChoice___init
 #define __pyx_n_s_RelativeWeightedChoice___init_2 __pyx_mstate_global->__pyx_n_s_RelativeWeightedChoice___init_2
 #define __pyx_n_s_RelativeWeightedChoice___init_3 __pyx_mstate_global->__pyx_n_s_RelativeWeightedChoice___init_3
 #define __pyx_kp_s_Relative_Weighted_Choice __pyx_mstate_global->__pyx_kp_s_Relative_Weighted_Choice
 #define __pyx_kp_u_Sample_size_k_is_larger_than_pop __pyx_mstate_global->__pyx_kp_u_Sample_size_k_is_larger_than_pop
 #define __pyx_n_s_TruffleShuffle __pyx_mstate_global->__pyx_n_s_TruffleShuffle
+#define __pyx_n_s_TruffleShuffle2 __pyx_mstate_global->__pyx_n_s_TruffleShuffle2
+#define __pyx_n_s_TruffleShuffle2___call __pyx_mstate_global->__pyx_n_s_TruffleShuffle2___call
+#define __pyx_n_s_TruffleShuffle2___init __pyx_mstate_global->__pyx_n_s_TruffleShuffle2___init
 #define __pyx_n_s_TruffleShuffle___call __pyx_mstate_global->__pyx_n_s_TruffleShuffle___call
 #define __pyx_n_s_TruffleShuffle___init __pyx_mstate_global->__pyx_n_s_TruffleShuffle___init
 #define __pyx_kp_s_Truffle_Shuffle_Produces_random __pyx_mstate_global->__pyx_kp_s_Truffle_Shuffle_Produces_random
 #define __pyx_n_s_TypeError __pyx_mstate_global->__pyx_n_s_TypeError
 #define __pyx_n_s_WeightedChoice __pyx_mstate_global->__pyx_n_s_WeightedChoice
 #define __pyx_n_s_WeightedChoice___call __pyx_mstate_global->__pyx_n_s_WeightedChoice___call
 #define __pyx_kp_s_Weighted_Choice_Base_Class_inte __pyx_mstate_global->__pyx_kp_s_Weighted_Choice_Base_Class_inte
 #define __pyx_n_s_ZeroCool __pyx_mstate_global->__pyx_n_s_ZeroCool
-#define __pyx_n_s__162 __pyx_mstate_global->__pyx_n_s__162
+#define __pyx_n_s__165 __pyx_mstate_global->__pyx_n_s__165
 #define __pyx_kp_u__2 __pyx_mstate_global->__pyx_kp_u__2
 #define __pyx_kp_u__3 __pyx_mstate_global->__pyx_kp_u__3
 #define __pyx_kp_u__4 __pyx_mstate_global->__pyx_kp_u__4
 #define __pyx_kp_u__5 __pyx_mstate_global->__pyx_kp_u__5
 #define __pyx_kp_u__6 __pyx_mstate_global->__pyx_kp_u__6
 #define __pyx_kp_u__7 __pyx_mstate_global->__pyx_kp_u__7
 #define __pyx_n_s_ability_dice __pyx_mstate_global->__pyx_n_s_ability_dice
@@ -4898,14 +4943,16 @@
 #define __pyx_n_s_genexpr __pyx_mstate_global->__pyx_n_s_genexpr
 #define __pyx_n_s_geometric_variate __pyx_mstate_global->__pyx_n_s_geometric_variate
 #define __pyx_n_s_get_answer __pyx_mstate_global->__pyx_n_s_get_answer
 #define __pyx_n_s_hi __pyx_mstate_global->__pyx_n_s_hi
 #define __pyx_n_s_high __pyx_mstate_global->__pyx_n_s_high
 #define __pyx_n_s_i __pyx_mstate_global->__pyx_n_s_i
 #define __pyx_n_s_import __pyx_mstate_global->__pyx_n_s_import
+#define __pyx_n_s_index __pyx_mstate_global->__pyx_n_s_index
+#define __pyx_n_u_index __pyx_mstate_global->__pyx_n_u_index
 #define __pyx_n_s_init __pyx_mstate_global->__pyx_n_s_init
 #define __pyx_n_s_init_subclass __pyx_mstate_global->__pyx_n_s_init_subclass
 #define __pyx_n_s_input __pyx_mstate_global->__pyx_n_s_input
 #define __pyx_n_s_int __pyx_mstate_global->__pyx_n_s_int
 #define __pyx_n_s_is_coroutine __pyx_mstate_global->__pyx_n_s_is_coroutine
 #define __pyx_kp_u_isenabled __pyx_mstate_global->__pyx_kp_u_isenabled
 #define __pyx_n_s_items __pyx_mstate_global->__pyx_n_s_items
@@ -4963,14 +5010,16 @@
 #define __pyx_n_s_normal_variate __pyx_mstate_global->__pyx_n_s_normal_variate
 #define __pyx_n_s_number __pyx_mstate_global->__pyx_n_s_number
 #define __pyx_n_s_number_of_trials __pyx_mstate_global->__pyx_n_s_number_of_trials
 #define __pyx_n_s_optimized_data __pyx_mstate_global->__pyx_n_s_optimized_data
 #define __pyx_n_s_options __pyx_mstate_global->__pyx_n_s_options
 #define __pyx_n_s_pareto_variate __pyx_mstate_global->__pyx_n_s_pareto_variate
 #define __pyx_n_s_percent_true __pyx_mstate_global->__pyx_n_s_percent_true
+#define __pyx_n_s_pivot __pyx_mstate_global->__pyx_n_s_pivot
+#define __pyx_n_u_pivot __pyx_mstate_global->__pyx_n_u_pivot
 #define __pyx_n_s_plus_or_minus __pyx_mstate_global->__pyx_n_s_plus_or_minus
 #define __pyx_n_s_plus_or_minus_gauss __pyx_mstate_global->__pyx_n_s_plus_or_minus_gauss
 #define __pyx_n_s_plus_or_minus_linear __pyx_mstate_global->__pyx_n_s_plus_or_minus_linear
 #define __pyx_n_s_poisson_variate __pyx_mstate_global->__pyx_n_s_poisson_variate
 #define __pyx_n_s_population __pyx_mstate_global->__pyx_n_s_population
 #define __pyx_n_s_prepare __pyx_mstate_global->__pyx_n_s_prepare
 #define __pyx_n_s_prev_weight __pyx_mstate_global->__pyx_n_s_prev_weight
@@ -5096,40 +5145,41 @@
 #define __pyx_tuple__83 __pyx_mstate_global->__pyx_tuple__83
 #define __pyx_tuple__85 __pyx_mstate_global->__pyx_tuple__85
 #define __pyx_tuple__86 __pyx_mstate_global->__pyx_tuple__86
 #define __pyx_tuple__88 __pyx_mstate_global->__pyx_tuple__88
 #define __pyx_tuple__90 __pyx_mstate_global->__pyx_tuple__90
 #define __pyx_tuple__91 __pyx_mstate_global->__pyx_tuple__91
 #define __pyx_tuple__94 __pyx_mstate_global->__pyx_tuple__94
+#define __pyx_tuple__97 __pyx_mstate_global->__pyx_tuple__97
 #define __pyx_codeobj__8 __pyx_mstate_global->__pyx_codeobj__8
-#define __pyx_tuple__111 __pyx_mstate_global->__pyx_tuple__111
-#define __pyx_tuple__112 __pyx_mstate_global->__pyx_tuple__112
 #define __pyx_tuple__114 __pyx_mstate_global->__pyx_tuple__114
 #define __pyx_tuple__115 __pyx_mstate_global->__pyx_tuple__115
 #define __pyx_tuple__117 __pyx_mstate_global->__pyx_tuple__117
 #define __pyx_tuple__118 __pyx_mstate_global->__pyx_tuple__118
-#define __pyx_tuple__119 __pyx_mstate_global->__pyx_tuple__119
+#define __pyx_tuple__120 __pyx_mstate_global->__pyx_tuple__120
 #define __pyx_tuple__121 __pyx_mstate_global->__pyx_tuple__121
-#define __pyx_tuple__123 __pyx_mstate_global->__pyx_tuple__123
-#define __pyx_tuple__125 __pyx_mstate_global->__pyx_tuple__125
+#define __pyx_tuple__122 __pyx_mstate_global->__pyx_tuple__122
+#define __pyx_tuple__124 __pyx_mstate_global->__pyx_tuple__124
+#define __pyx_tuple__126 __pyx_mstate_global->__pyx_tuple__126
 #define __pyx_tuple__128 __pyx_mstate_global->__pyx_tuple__128
-#define __pyx_tuple__130 __pyx_mstate_global->__pyx_tuple__130
-#define __pyx_tuple__132 __pyx_mstate_global->__pyx_tuple__132
-#define __pyx_tuple__134 __pyx_mstate_global->__pyx_tuple__134
-#define __pyx_tuple__136 __pyx_mstate_global->__pyx_tuple__136
-#define __pyx_tuple__138 __pyx_mstate_global->__pyx_tuple__138
+#define __pyx_tuple__131 __pyx_mstate_global->__pyx_tuple__131
+#define __pyx_tuple__133 __pyx_mstate_global->__pyx_tuple__133
+#define __pyx_tuple__135 __pyx_mstate_global->__pyx_tuple__135
+#define __pyx_tuple__137 __pyx_mstate_global->__pyx_tuple__137
+#define __pyx_tuple__139 __pyx_mstate_global->__pyx_tuple__139
 #define __pyx_tuple__141 __pyx_mstate_global->__pyx_tuple__141
-#define __pyx_tuple__143 __pyx_mstate_global->__pyx_tuple__143
-#define __pyx_tuple__145 __pyx_mstate_global->__pyx_tuple__145
-#define __pyx_tuple__147 __pyx_mstate_global->__pyx_tuple__147
+#define __pyx_tuple__144 __pyx_mstate_global->__pyx_tuple__144
+#define __pyx_tuple__146 __pyx_mstate_global->__pyx_tuple__146
+#define __pyx_tuple__148 __pyx_mstate_global->__pyx_tuple__148
 #define __pyx_tuple__150 __pyx_mstate_global->__pyx_tuple__150
-#define __pyx_tuple__152 __pyx_mstate_global->__pyx_tuple__152
-#define __pyx_tuple__154 __pyx_mstate_global->__pyx_tuple__154
-#define __pyx_tuple__156 __pyx_mstate_global->__pyx_tuple__156
+#define __pyx_tuple__153 __pyx_mstate_global->__pyx_tuple__153
+#define __pyx_tuple__155 __pyx_mstate_global->__pyx_tuple__155
+#define __pyx_tuple__157 __pyx_mstate_global->__pyx_tuple__157
 #define __pyx_tuple__159 __pyx_mstate_global->__pyx_tuple__159
+#define __pyx_tuple__162 __pyx_mstate_global->__pyx_tuple__162
 #define __pyx_codeobj__10 __pyx_mstate_global->__pyx_codeobj__10
 #define __pyx_codeobj__11 __pyx_mstate_global->__pyx_codeobj__11
 #define __pyx_codeobj__12 __pyx_mstate_global->__pyx_codeobj__12
 #define __pyx_codeobj__13 __pyx_mstate_global->__pyx_codeobj__13
 #define __pyx_codeobj__14 __pyx_mstate_global->__pyx_codeobj__14
 #define __pyx_codeobj__15 __pyx_mstate_global->__pyx_codeobj__15
 #define __pyx_codeobj__16 __pyx_mstate_global->__pyx_codeobj__16
@@ -5179,54 +5229,56 @@
 #define __pyx_codeobj__84 __pyx_mstate_global->__pyx_codeobj__84
 #define __pyx_codeobj__87 __pyx_mstate_global->__pyx_codeobj__87
 #define __pyx_codeobj__89 __pyx_mstate_global->__pyx_codeobj__89
 #define __pyx_codeobj__92 __pyx_mstate_global->__pyx_codeobj__92
 #define __pyx_codeobj__93 __pyx_mstate_global->__pyx_codeobj__93
 #define __pyx_codeobj__95 __pyx_mstate_global->__pyx_codeobj__95
 #define __pyx_codeobj__96 __pyx_mstate_global->__pyx_codeobj__96
-#define __pyx_codeobj__97 __pyx_mstate_global->__pyx_codeobj__97
 #define __pyx_codeobj__98 __pyx_mstate_global->__pyx_codeobj__98
 #define __pyx_codeobj__99 __pyx_mstate_global->__pyx_codeobj__99
 #define __pyx_codeobj__100 __pyx_mstate_global->__pyx_codeobj__100
 #define __pyx_codeobj__101 __pyx_mstate_global->__pyx_codeobj__101
 #define __pyx_codeobj__102 __pyx_mstate_global->__pyx_codeobj__102
 #define __pyx_codeobj__103 __pyx_mstate_global->__pyx_codeobj__103
 #define __pyx_codeobj__104 __pyx_mstate_global->__pyx_codeobj__104
 #define __pyx_codeobj__105 __pyx_mstate_global->__pyx_codeobj__105
 #define __pyx_codeobj__106 __pyx_mstate_global->__pyx_codeobj__106
 #define __pyx_codeobj__107 __pyx_mstate_global->__pyx_codeobj__107
 #define __pyx_codeobj__108 __pyx_mstate_global->__pyx_codeobj__108
 #define __pyx_codeobj__109 __pyx_mstate_global->__pyx_codeobj__109
 #define __pyx_codeobj__110 __pyx_mstate_global->__pyx_codeobj__110
+#define __pyx_codeobj__111 __pyx_mstate_global->__pyx_codeobj__111
+#define __pyx_codeobj__112 __pyx_mstate_global->__pyx_codeobj__112
 #define __pyx_codeobj__113 __pyx_mstate_global->__pyx_codeobj__113
 #define __pyx_codeobj__116 __pyx_mstate_global->__pyx_codeobj__116
-#define __pyx_codeobj__120 __pyx_mstate_global->__pyx_codeobj__120
-#define __pyx_codeobj__122 __pyx_mstate_global->__pyx_codeobj__122
-#define __pyx_codeobj__124 __pyx_mstate_global->__pyx_codeobj__124
-#define __pyx_codeobj__126 __pyx_mstate_global->__pyx_codeobj__126
+#define __pyx_codeobj__119 __pyx_mstate_global->__pyx_codeobj__119
+#define __pyx_codeobj__123 __pyx_mstate_global->__pyx_codeobj__123
+#define __pyx_codeobj__125 __pyx_mstate_global->__pyx_codeobj__125
 #define __pyx_codeobj__127 __pyx_mstate_global->__pyx_codeobj__127
 #define __pyx_codeobj__129 __pyx_mstate_global->__pyx_codeobj__129
-#define __pyx_codeobj__131 __pyx_mstate_global->__pyx_codeobj__131
-#define __pyx_codeobj__133 __pyx_mstate_global->__pyx_codeobj__133
-#define __pyx_codeobj__135 __pyx_mstate_global->__pyx_codeobj__135
-#define __pyx_codeobj__137 __pyx_mstate_global->__pyx_codeobj__137
-#define __pyx_codeobj__139 __pyx_mstate_global->__pyx_codeobj__139
+#define __pyx_codeobj__130 __pyx_mstate_global->__pyx_codeobj__130
+#define __pyx_codeobj__132 __pyx_mstate_global->__pyx_codeobj__132
+#define __pyx_codeobj__134 __pyx_mstate_global->__pyx_codeobj__134
+#define __pyx_codeobj__136 __pyx_mstate_global->__pyx_codeobj__136
+#define __pyx_codeobj__138 __pyx_mstate_global->__pyx_codeobj__138
 #define __pyx_codeobj__140 __pyx_mstate_global->__pyx_codeobj__140
 #define __pyx_codeobj__142 __pyx_mstate_global->__pyx_codeobj__142
-#define __pyx_codeobj__144 __pyx_mstate_global->__pyx_codeobj__144
-#define __pyx_codeobj__146 __pyx_mstate_global->__pyx_codeobj__146
-#define __pyx_codeobj__148 __pyx_mstate_global->__pyx_codeobj__148
+#define __pyx_codeobj__143 __pyx_mstate_global->__pyx_codeobj__143
+#define __pyx_codeobj__145 __pyx_mstate_global->__pyx_codeobj__145
+#define __pyx_codeobj__147 __pyx_mstate_global->__pyx_codeobj__147
 #define __pyx_codeobj__149 __pyx_mstate_global->__pyx_codeobj__149
 #define __pyx_codeobj__151 __pyx_mstate_global->__pyx_codeobj__151
-#define __pyx_codeobj__153 __pyx_mstate_global->__pyx_codeobj__153
-#define __pyx_codeobj__155 __pyx_mstate_global->__pyx_codeobj__155
-#define __pyx_codeobj__157 __pyx_mstate_global->__pyx_codeobj__157
+#define __pyx_codeobj__152 __pyx_mstate_global->__pyx_codeobj__152
+#define __pyx_codeobj__154 __pyx_mstate_global->__pyx_codeobj__154
+#define __pyx_codeobj__156 __pyx_mstate_global->__pyx_codeobj__156
 #define __pyx_codeobj__158 __pyx_mstate_global->__pyx_codeobj__158
 #define __pyx_codeobj__160 __pyx_mstate_global->__pyx_codeobj__160
 #define __pyx_codeobj__161 __pyx_mstate_global->__pyx_codeobj__161
+#define __pyx_codeobj__163 __pyx_mstate_global->__pyx_codeobj__163
+#define __pyx_codeobj__164 __pyx_mstate_global->__pyx_codeobj__164
 /* #### Code section: module_code ### */
 
 /* "Fortuna.pyx":70
  * 
  * 
  * def storm_version() -> str:             # <<<<<<<<<<<<<<
  *     """ Current version of Storm """
@@ -14682,15 +14734,528 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "Fortuna.pyx":583
+/* "Fortuna.pyx":555
+ *     __slots__ = ("flat", "data", "size", "pivot", "index")
+ * 
+ *     def __init__(self, collection: Iterable, flat: bool = True):             # <<<<<<<<<<<<<<
+ *         self.flat = flat
+ *         self.data = list(collection) if isinstance(collection, Iterator) else collection
+ */
+
+/* Python wrapper */
+static PyObject *__pyx_pw_7Fortuna_15TruffleShuffle2_1__init__(PyObject *__pyx_self, 
+#if CYTHON_METH_FASTCALL
+PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
+#else
+PyObject *__pyx_args, PyObject *__pyx_kwds
+#endif
+); /*proto*/
+PyDoc_STRVAR(__pyx_doc_7Fortuna_15TruffleShuffle2___init__, "TruffleShuffle2.__init__(self, collection: Iterable, flat: bool = True)");
+static PyMethodDef __pyx_mdef_7Fortuna_15TruffleShuffle2_1__init__ = {"__init__", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_7Fortuna_15TruffleShuffle2_1__init__, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_7Fortuna_15TruffleShuffle2___init__};
+static PyObject *__pyx_pw_7Fortuna_15TruffleShuffle2_1__init__(PyObject *__pyx_self, 
+#if CYTHON_METH_FASTCALL
+PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
+#else
+PyObject *__pyx_args, PyObject *__pyx_kwds
+#endif
+) {
+  PyObject *__pyx_v_self = 0;
+  PyObject *__pyx_v_collection = 0;
+  PyObject *__pyx_v_flat = 0;
+  #if !CYTHON_METH_FASTCALL
+  CYTHON_UNUSED Py_ssize_t __pyx_nargs;
+  #endif
+  CYTHON_UNUSED PyObject *const *__pyx_kwvalues;
+  PyObject* values[3] = {0,0,0};
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  PyObject *__pyx_r = 0;
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("__init__ (wrapper)", 0);
+  #if !CYTHON_METH_FASTCALL
+  #if CYTHON_ASSUME_SAFE_MACROS
+  __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
+  #else
+  __pyx_nargs = PyTuple_Size(__pyx_args); if (unlikely(__pyx_nargs < 0)) return NULL;
+  #endif
+  #endif
+  __pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
+  {
+    PyObject **__pyx_pyargnames[] = {&__pyx_n_s_self,&__pyx_n_s_collection,&__pyx_n_s_flat,0};
+    values[2] = __Pyx_Arg_NewRef_FASTCALL(((PyObject *)((PyObject *)Py_True)));
+    if (__pyx_kwds) {
+      Py_ssize_t kw_args;
+      switch (__pyx_nargs) {
+        case  3: values[2] = __Pyx_Arg_FASTCALL(__pyx_args, 2);
+        CYTHON_FALLTHROUGH;
+        case  2: values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
+        CYTHON_FALLTHROUGH;
+        case  1: values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
+        CYTHON_FALLTHROUGH;
+        case  0: break;
+        default: goto __pyx_L5_argtuple_error;
+      }
+      kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
+      switch (__pyx_nargs) {
+        case  0:
+        if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_self)) != 0)) {
+          (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
+          kw_args--;
+        }
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 555, __pyx_L3_error)
+        else goto __pyx_L5_argtuple_error;
+        CYTHON_FALLTHROUGH;
+        case  1:
+        if (likely((values[1] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_collection)) != 0)) {
+          (void)__Pyx_Arg_NewRef_FASTCALL(values[1]);
+          kw_args--;
+        }
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 555, __pyx_L3_error)
+        else {
+          __Pyx_RaiseArgtupleInvalid("__init__", 0, 2, 3, 1); __PYX_ERR(0, 555, __pyx_L3_error)
+        }
+        CYTHON_FALLTHROUGH;
+        case  2:
+        if (kw_args > 0) {
+          PyObject* value = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_flat);
+          if (value) { values[2] = __Pyx_Arg_NewRef_FASTCALL(value); kw_args--; }
+          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 555, __pyx_L3_error)
+        }
+      }
+      if (unlikely(kw_args > 0)) {
+        const Py_ssize_t kwd_pos_args = __pyx_nargs;
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "__init__") < 0)) __PYX_ERR(0, 555, __pyx_L3_error)
+      }
+    } else {
+      switch (__pyx_nargs) {
+        case  3: values[2] = __Pyx_Arg_FASTCALL(__pyx_args, 2);
+        CYTHON_FALLTHROUGH;
+        case  2: values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
+        values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
+        break;
+        default: goto __pyx_L5_argtuple_error;
+      }
+    }
+    __pyx_v_self = values[0];
+    __pyx_v_collection = values[1];
+    __pyx_v_flat = values[2];
+  }
+  goto __pyx_L6_skip;
+  __pyx_L5_argtuple_error:;
+  __Pyx_RaiseArgtupleInvalid("__init__", 0, 2, 3, __pyx_nargs); __PYX_ERR(0, 555, __pyx_L3_error)
+  __pyx_L6_skip:;
+  goto __pyx_L4_argument_unpacking_done;
+  __pyx_L3_error:;
+  {
+    Py_ssize_t __pyx_temp;
+    for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
+      __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
+    }
+  }
+  __Pyx_AddTraceback("Fortuna.TruffleShuffle2.__init__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_RefNannyFinishContext();
+  return NULL;
+  __pyx_L4_argument_unpacking_done:;
+  __pyx_r = __pyx_pf_7Fortuna_15TruffleShuffle2___init__(__pyx_self, __pyx_v_self, __pyx_v_collection, __pyx_v_flat);
+
+  /* function exit code */
+  {
+    Py_ssize_t __pyx_temp;
+    for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
+      __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
+    }
+  }
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+static PyObject *__pyx_pf_7Fortuna_15TruffleShuffle2___init__(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_collection, PyObject *__pyx_v_flat) {
+  PyObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  PyObject *__pyx_t_1 = NULL;
+  PyObject *__pyx_t_2 = NULL;
+  int __pyx_t_3;
+  Py_ssize_t __pyx_t_4;
+  PyObject *__pyx_t_5 = NULL;
+  PyObject *__pyx_t_6 = NULL;
+  int __pyx_t_7;
+  PY_LONG_LONG __pyx_t_8;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("__init__", 1);
+
+  /* "Fortuna.pyx":556
+ * 
+ *     def __init__(self, collection: Iterable, flat: bool = True):
+ *         self.flat = flat             # <<<<<<<<<<<<<<
+ *         self.data = list(collection) if isinstance(collection, Iterator) else collection
+ *         self.size = len(self.data)
+ */
+  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_flat, __pyx_v_flat) < 0) __PYX_ERR(0, 556, __pyx_L1_error)
+
+  /* "Fortuna.pyx":557
+ *     def __init__(self, collection: Iterable, flat: bool = True):
+ *         self.flat = flat
+ *         self.data = list(collection) if isinstance(collection, Iterator) else collection             # <<<<<<<<<<<<<<
+ *         self.size = len(self.data)
+ *         self.pivot = int(sqrt(self.size))
+ */
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_Iterator); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 557, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __pyx_t_3 = PyObject_IsInstance(__pyx_v_collection, __pyx_t_2); if (unlikely(__pyx_t_3 == ((int)-1))) __PYX_ERR(0, 557, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  if (__pyx_t_3) {
+    __pyx_t_2 = PySequence_List(__pyx_v_collection); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 557, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_1 = __pyx_t_2;
+    __pyx_t_2 = 0;
+  } else {
+    __Pyx_INCREF(__pyx_v_collection);
+    __pyx_t_1 = __pyx_v_collection;
+  }
+  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_data, __pyx_t_1) < 0) __PYX_ERR(0, 557, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+
+  /* "Fortuna.pyx":558
+ *         self.flat = flat
+ *         self.data = list(collection) if isinstance(collection, Iterator) else collection
+ *         self.size = len(self.data)             # <<<<<<<<<<<<<<
+ *         self.pivot = int(sqrt(self.size))
+ *         self.index = _random_index(self.size)
+ */
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_data); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 558, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_4 = PyObject_Length(__pyx_t_1); if (unlikely(__pyx_t_4 == ((Py_ssize_t)-1))) __PYX_ERR(0, 558, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_t_1 = PyInt_FromSsize_t(__pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 558, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_size, __pyx_t_1) < 0) __PYX_ERR(0, 558, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+
+  /* "Fortuna.pyx":559
+ *         self.data = list(collection) if isinstance(collection, Iterator) else collection
+ *         self.size = len(self.data)
+ *         self.pivot = int(sqrt(self.size))             # <<<<<<<<<<<<<<
+ *         self.index = _random_index(self.size)
+ * 
+ */
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_sqrt); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 559, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_size); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 559, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
+  __pyx_t_6 = NULL;
+  __pyx_t_7 = 0;
+  #if CYTHON_UNPACK_METHODS
+  if (unlikely(PyMethod_Check(__pyx_t_2))) {
+    __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_2);
+    if (likely(__pyx_t_6)) {
+      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
+      __Pyx_INCREF(__pyx_t_6);
+      __Pyx_INCREF(function);
+      __Pyx_DECREF_SET(__pyx_t_2, function);
+      __pyx_t_7 = 1;
+    }
+  }
+  #endif
+  {
+    PyObject *__pyx_callargs[2] = {__pyx_t_6, __pyx_t_5};
+    __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_2, __pyx_callargs+1-__pyx_t_7, 1+__pyx_t_7);
+    __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
+    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 559, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  }
+  __pyx_t_2 = __Pyx_PyNumber_Int(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 559, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_pivot, __pyx_t_2) < 0) __PYX_ERR(0, 559, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+
+  /* "Fortuna.pyx":560
+ *         self.size = len(self.data)
+ *         self.pivot = int(sqrt(self.size))
+ *         self.index = _random_index(self.size)             # <<<<<<<<<<<<<<
+ * 
+ *     def __call__(self, *args, **kwargs):
+ */
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_size); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 560, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __pyx_t_8 = __Pyx_PyInt_As_PY_LONG_LONG(__pyx_t_2); if (unlikely((__pyx_t_8 == (PY_LONG_LONG)-1) && PyErr_Occurred())) __PYX_ERR(0, 560, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __pyx_t_2 = __Pyx_PyInt_From_PY_LONG_LONG(Storm::GetIndex::random_index(__pyx_t_8)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 560, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_index, __pyx_t_2) < 0) __PYX_ERR(0, 560, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+
+  /* "Fortuna.pyx":555
+ *     __slots__ = ("flat", "data", "size", "pivot", "index")
+ * 
+ *     def __init__(self, collection: Iterable, flat: bool = True):             # <<<<<<<<<<<<<<
+ *         self.flat = flat
+ *         self.data = list(collection) if isinstance(collection, Iterator) else collection
+ */
+
+  /* function exit code */
+  __pyx_r = Py_None; __Pyx_INCREF(Py_None);
+  goto __pyx_L0;
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_1);
+  __Pyx_XDECREF(__pyx_t_2);
+  __Pyx_XDECREF(__pyx_t_5);
+  __Pyx_XDECREF(__pyx_t_6);
+  __Pyx_AddTraceback("Fortuna.TruffleShuffle2.__init__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = NULL;
+  __pyx_L0:;
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "Fortuna.pyx":562
+ *         self.index = _random_index(self.size)
+ * 
+ *     def __call__(self, *args, **kwargs):             # <<<<<<<<<<<<<<
+ *         self.index = (self.index + 1 + _front_poisson(self.pivot)) % self.size
+ *         return flatten(self.data[self.index], *args, flat=self.flat, **kwargs)
+ */
+
+/* Python wrapper */
+static PyObject *__pyx_pw_7Fortuna_15TruffleShuffle2_3__call__(PyObject *__pyx_self, 
+#if CYTHON_METH_FASTCALL
+PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
+#else
+PyObject *__pyx_args, PyObject *__pyx_kwds
+#endif
+); /*proto*/
+PyDoc_STRVAR(__pyx_doc_7Fortuna_15TruffleShuffle2_2__call__, "TruffleShuffle2.__call__(self, *args, **kwargs)");
+static PyMethodDef __pyx_mdef_7Fortuna_15TruffleShuffle2_3__call__ = {"__call__", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_7Fortuna_15TruffleShuffle2_3__call__, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_7Fortuna_15TruffleShuffle2_2__call__};
+static PyObject *__pyx_pw_7Fortuna_15TruffleShuffle2_3__call__(PyObject *__pyx_self, 
+#if CYTHON_METH_FASTCALL
+PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
+#else
+PyObject *__pyx_args, PyObject *__pyx_kwds
+#endif
+) {
+  PyObject *__pyx_v_self = 0;
+  PyObject *__pyx_v_args = 0;
+  PyObject *__pyx_v_kwargs = 0;
+  #if !CYTHON_METH_FASTCALL
+  CYTHON_UNUSED Py_ssize_t __pyx_nargs;
+  #endif
+  CYTHON_UNUSED PyObject *const *__pyx_kwvalues;
+  PyObject* values[1] = {0};
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  PyObject *__pyx_r = 0;
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("__call__ (wrapper)", 0);
+  #if !CYTHON_METH_FASTCALL
+  #if CYTHON_ASSUME_SAFE_MACROS
+  __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
+  #else
+  __pyx_nargs = PyTuple_Size(__pyx_args); if (unlikely(__pyx_nargs < 0)) return NULL;
+  #endif
+  #endif
+  __pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
+  __pyx_v_kwargs = PyDict_New(); if (unlikely(!__pyx_v_kwargs)) return NULL;
+  __Pyx_GOTREF(__pyx_v_kwargs);
+  __pyx_v_args = __Pyx_ArgsSlice_FASTCALL(__pyx_args, 1, __pyx_nargs);
+  if (unlikely(!__pyx_v_args)) {
+    __Pyx_DECREF(__pyx_v_kwargs); __pyx_v_kwargs = 0;
+    __Pyx_RefNannyFinishContext();
+    return NULL;
+  }
+  __Pyx_GOTREF(__pyx_v_args);
+  {
+    PyObject **__pyx_pyargnames[] = {&__pyx_n_s_self,0};
+    if (__pyx_kwds) {
+      Py_ssize_t kw_args;
+      switch (__pyx_nargs) {
+        default:
+        case  1: values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
+        CYTHON_FALLTHROUGH;
+        case  0: break;
+      }
+      kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
+      switch (__pyx_nargs) {
+        case  0:
+        if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_self)) != 0)) {
+          (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
+          kw_args--;
+        }
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 562, __pyx_L3_error)
+        else goto __pyx_L5_argtuple_error;
+      }
+      if (unlikely(kw_args > 0)) {
+        const Py_ssize_t kwd_pos_args = __pyx_nargs;
+        const Py_ssize_t used_pos_args = (kwd_pos_args < 1) ? kwd_pos_args : 1;
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, __pyx_v_kwargs, values + 0, used_pos_args, "__call__") < 0)) __PYX_ERR(0, 562, __pyx_L3_error)
+      }
+    } else if (unlikely(__pyx_nargs < 1)) {
+      goto __pyx_L5_argtuple_error;
+    } else {
+      values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
+    }
+    __pyx_v_self = values[0];
+  }
+  goto __pyx_L6_skip;
+  __pyx_L5_argtuple_error:;
+  __Pyx_RaiseArgtupleInvalid("__call__", 0, 1, 1, __pyx_nargs); __PYX_ERR(0, 562, __pyx_L3_error)
+  __pyx_L6_skip:;
+  goto __pyx_L4_argument_unpacking_done;
+  __pyx_L3_error:;
+  {
+    Py_ssize_t __pyx_temp;
+    for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
+      __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
+    }
+  }
+  __Pyx_DECREF(__pyx_v_args); __pyx_v_args = 0;
+  __Pyx_DECREF(__pyx_v_kwargs); __pyx_v_kwargs = 0;
+  __Pyx_AddTraceback("Fortuna.TruffleShuffle2.__call__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_RefNannyFinishContext();
+  return NULL;
+  __pyx_L4_argument_unpacking_done:;
+  __pyx_r = __pyx_pf_7Fortuna_15TruffleShuffle2_2__call__(__pyx_self, __pyx_v_self, __pyx_v_args, __pyx_v_kwargs);
+
+  /* function exit code */
+  __Pyx_DECREF(__pyx_v_args);
+  __Pyx_DECREF(__pyx_v_kwargs);
+  {
+    Py_ssize_t __pyx_temp;
+    for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
+      __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
+    }
+  }
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+static PyObject *__pyx_pf_7Fortuna_15TruffleShuffle2_2__call__(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_args, PyObject *__pyx_v_kwargs) {
+  PyObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  PyObject *__pyx_t_1 = NULL;
+  PyObject *__pyx_t_2 = NULL;
+  PY_LONG_LONG __pyx_t_3;
+  PyObject *__pyx_t_4 = NULL;
+  PyObject *__pyx_t_5 = NULL;
+  PyObject *__pyx_t_6 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("__call__", 1);
+
+  /* "Fortuna.pyx":563
+ * 
+ *     def __call__(self, *args, **kwargs):
+ *         self.index = (self.index + 1 + _front_poisson(self.pivot)) % self.size             # <<<<<<<<<<<<<<
+ *         return flatten(self.data[self.index], *args, flat=self.flat, **kwargs)
+ * 
+ */
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_index); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 563, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_2 = __Pyx_PyInt_AddObjC(__pyx_t_1, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 563, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_pivot); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 563, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_3 = __Pyx_PyInt_As_PY_LONG_LONG(__pyx_t_1); if (unlikely((__pyx_t_3 == (PY_LONG_LONG)-1) && PyErr_Occurred())) __PYX_ERR(0, 563, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_t_1 = __Pyx_PyInt_From_PY_LONG_LONG(Storm::GetIndex::front_poisson(__pyx_t_3)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 563, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_4 = PyNumber_Add(__pyx_t_2, __pyx_t_1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 563, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_size); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 563, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_2 = PyNumber_Remainder(__pyx_t_4, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 563, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_index, __pyx_t_2) < 0) __PYX_ERR(0, 563, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+
+  /* "Fortuna.pyx":564
+ *     def __call__(self, *args, **kwargs):
+ *         self.index = (self.index + 1 + _front_poisson(self.pivot)) % self.size
+ *         return flatten(self.data[self.index], *args, flat=self.flat, **kwargs)             # <<<<<<<<<<<<<<
+ * 
+ * 
+ */
+  __Pyx_XDECREF(__pyx_r);
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_flatten); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 564, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_data); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 564, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_index); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 564, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __pyx_t_5 = __Pyx_PyObject_GetItem(__pyx_t_1, __pyx_t_4); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 564, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 564, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __Pyx_GIVEREF(__pyx_t_5);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_5)) __PYX_ERR(0, 564, __pyx_L1_error);
+  __pyx_t_5 = 0;
+  __pyx_t_5 = PyNumber_Add(__pyx_t_4, __pyx_v_args); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 564, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
+  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 564, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_flat); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 564, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_6);
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_flat, __pyx_t_6) < 0) __PYX_ERR(0, 564, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+  __pyx_t_4 = __pyx_t_1;
+  __pyx_t_1 = 0;
+  if (__Pyx_MergeKeywords(__pyx_t_4, __pyx_v_kwargs) < 0) __PYX_ERR(0, 564, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_5, __pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 564, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  __pyx_r = __pyx_t_1;
+  __pyx_t_1 = 0;
+  goto __pyx_L0;
+
+  /* "Fortuna.pyx":562
+ *         self.index = _random_index(self.size)
+ * 
+ *     def __call__(self, *args, **kwargs):             # <<<<<<<<<<<<<<
+ *         self.index = (self.index + 1 + _front_poisson(self.pivot)) % self.size
+ *         return flatten(self.data[self.index], *args, flat=self.flat, **kwargs)
+ */
+
+  /* function exit code */
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_1);
+  __Pyx_XDECREF(__pyx_t_2);
+  __Pyx_XDECREF(__pyx_t_4);
+  __Pyx_XDECREF(__pyx_t_5);
+  __Pyx_XDECREF(__pyx_t_6);
+  __Pyx_AddTraceback("Fortuna.TruffleShuffle2.__call__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = NULL;
+  __pyx_L0:;
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "Fortuna.pyx":598
  *     __slots__ = ("flat", "data", "rotate_size")
  * 
  *     def __init__(self, collection: Iterable, flat: bool = True):             # <<<<<<<<<<<<<<
  *         self.flat = flat
  *         data = list(collection)
  */
 
@@ -14751,37 +15316,37 @@
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_self)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 583, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 598, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_collection)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[1]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 583, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 598, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("__init__", 0, 2, 3, 1); __PYX_ERR(0, 583, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__init__", 0, 2, 3, 1); __PYX_ERR(0, 598, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (kw_args > 0) {
           PyObject* value = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_flat);
           if (value) { values[2] = __Pyx_Arg_NewRef_FASTCALL(value); kw_args--; }
-          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 583, __pyx_L3_error)
+          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 598, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "__init__") < 0)) __PYX_ERR(0, 583, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "__init__") < 0)) __PYX_ERR(0, 598, __pyx_L3_error)
       }
     } else {
       switch (__pyx_nargs) {
         case  3: values[2] = __Pyx_Arg_FASTCALL(__pyx_args, 2);
         CYTHON_FALLTHROUGH;
         case  2: values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
         values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
@@ -14791,15 +15356,15 @@
     }
     __pyx_v_self = values[0];
     __pyx_v_collection = values[1];
     __pyx_v_flat = values[2];
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__init__", 0, 2, 3, __pyx_nargs); __PYX_ERR(0, 583, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__init__", 0, 2, 3, __pyx_nargs); __PYX_ERR(0, 598, __pyx_L3_error)
   __pyx_L6_skip:;
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
@@ -14833,43 +15398,43 @@
   Py_ssize_t __pyx_t_5;
   PyObject *__pyx_t_6 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__init__", 1);
 
-  /* "Fortuna.pyx":584
+  /* "Fortuna.pyx":599
  * 
  *     def __init__(self, collection: Iterable, flat: bool = True):
  *         self.flat = flat             # <<<<<<<<<<<<<<
  *         data = list(collection)
  *         shuffle(data)
  */
-  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_flat, __pyx_v_flat) < 0) __PYX_ERR(0, 584, __pyx_L1_error)
+  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_flat, __pyx_v_flat) < 0) __PYX_ERR(0, 599, __pyx_L1_error)
 
-  /* "Fortuna.pyx":585
+  /* "Fortuna.pyx":600
  *     def __init__(self, collection: Iterable, flat: bool = True):
  *         self.flat = flat
  *         data = list(collection)             # <<<<<<<<<<<<<<
  *         shuffle(data)
  *         self.data = deque(data)
  */
-  __pyx_t_1 = PySequence_List(__pyx_v_collection); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 585, __pyx_L1_error)
+  __pyx_t_1 = PySequence_List(__pyx_v_collection); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 600, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_data = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "Fortuna.pyx":586
+  /* "Fortuna.pyx":601
  *         self.flat = flat
  *         data = list(collection)
  *         shuffle(data)             # <<<<<<<<<<<<<<
  *         self.data = deque(data)
  *         self.rotate_size = int(sqrt(len(self.data)))
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_shuffle); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 586, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_shuffle); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 601, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
   __pyx_t_4 = 0;
   #if CYTHON_UNPACK_METHODS
   if (unlikely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
@@ -14881,28 +15446,28 @@
     }
   }
   #endif
   {
     PyObject *__pyx_callargs[2] = {__pyx_t_3, __pyx_v_data};
     __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_2, __pyx_callargs+1-__pyx_t_4, 1+__pyx_t_4);
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 586, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 601, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   }
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "Fortuna.pyx":587
+  /* "Fortuna.pyx":602
  *         data = list(collection)
  *         shuffle(data)
  *         self.data = deque(data)             # <<<<<<<<<<<<<<
  *         self.rotate_size = int(sqrt(len(self.data)))
  * 
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_deque); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 587, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_deque); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 602, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
   __pyx_t_4 = 0;
   #if CYTHON_UNPACK_METHODS
   if (unlikely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
@@ -14914,35 +15479,35 @@
     }
   }
   #endif
   {
     PyObject *__pyx_callargs[2] = {__pyx_t_3, __pyx_v_data};
     __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_2, __pyx_callargs+1-__pyx_t_4, 1+__pyx_t_4);
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 587, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 602, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   }
-  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_data, __pyx_t_1) < 0) __PYX_ERR(0, 587, __pyx_L1_error)
+  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_data, __pyx_t_1) < 0) __PYX_ERR(0, 602, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "Fortuna.pyx":588
+  /* "Fortuna.pyx":603
  *         shuffle(data)
  *         self.data = deque(data)
  *         self.rotate_size = int(sqrt(len(self.data)))             # <<<<<<<<<<<<<<
  * 
  *     def __call__(self, *args, **kwargs):
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_sqrt); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 588, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_sqrt); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 603, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_data); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 588, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_data); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 603, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_5 = PyObject_Length(__pyx_t_3); if (unlikely(__pyx_t_5 == ((Py_ssize_t)-1))) __PYX_ERR(0, 588, __pyx_L1_error)
+  __pyx_t_5 = PyObject_Length(__pyx_t_3); if (unlikely(__pyx_t_5 == ((Py_ssize_t)-1))) __PYX_ERR(0, 603, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = PyInt_FromSsize_t(__pyx_t_5); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 588, __pyx_L1_error)
+  __pyx_t_3 = PyInt_FromSsize_t(__pyx_t_5); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 603, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_6 = NULL;
   __pyx_t_4 = 0;
   #if CYTHON_UNPACK_METHODS
   if (unlikely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_6)) {
@@ -14955,25 +15520,25 @@
   }
   #endif
   {
     PyObject *__pyx_callargs[2] = {__pyx_t_6, __pyx_t_3};
     __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_2, __pyx_callargs+1-__pyx_t_4, 1+__pyx_t_4);
     __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 588, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 603, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   }
-  __pyx_t_2 = __Pyx_PyNumber_Int(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 588, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyNumber_Int(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 603, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_rotate_size, __pyx_t_2) < 0) __PYX_ERR(0, 588, __pyx_L1_error)
+  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_rotate_size, __pyx_t_2) < 0) __PYX_ERR(0, 603, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "Fortuna.pyx":583
+  /* "Fortuna.pyx":598
  *     __slots__ = ("flat", "data", "rotate_size")
  * 
  *     def __init__(self, collection: Iterable, flat: bool = True):             # <<<<<<<<<<<<<<
  *         self.flat = flat
  *         data = list(collection)
  */
 
@@ -14990,15 +15555,15 @@
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_data);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "Fortuna.pyx":590
+/* "Fortuna.pyx":605
  *         self.rotate_size = int(sqrt(len(self.data)))
  * 
  *     def __call__(self, *args, **kwargs):             # <<<<<<<<<<<<<<
  *         self.data.rotate(1 + _front_poisson(self.rotate_size))
  *         return flatten(self.data[-1], *args, flat=self.flat, **kwargs)
  */
 
@@ -15063,32 +15628,32 @@
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_self)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 590, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 605, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
         const Py_ssize_t used_pos_args = (kwd_pos_args < 1) ? kwd_pos_args : 1;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, __pyx_v_kwargs, values + 0, used_pos_args, "__call__") < 0)) __PYX_ERR(0, 590, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, __pyx_v_kwargs, values + 0, used_pos_args, "__call__") < 0)) __PYX_ERR(0, 605, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs < 1)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
     }
     __pyx_v_self = values[0];
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__call__", 0, 1, 1, __pyx_nargs); __PYX_ERR(0, 590, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__call__", 0, 1, 1, __pyx_nargs); __PYX_ERR(0, 605, __pyx_L3_error)
   __pyx_L6_skip:;
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
@@ -15126,31 +15691,31 @@
   int __pyx_t_6;
   PyObject *__pyx_t_7 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__call__", 1);
 
-  /* "Fortuna.pyx":591
+  /* "Fortuna.pyx":606
  * 
  *     def __call__(self, *args, **kwargs):
  *         self.data.rotate(1 + _front_poisson(self.rotate_size))             # <<<<<<<<<<<<<<
  *         return flatten(self.data[-1], *args, flat=self.flat, **kwargs)
  * 
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_data); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 591, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_data); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 606, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_rotate); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 591, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_rotate); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 606, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_rotate_size); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 591, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_rotate_size); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 606, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_4 = __Pyx_PyInt_As_PY_LONG_LONG(__pyx_t_2); if (unlikely((__pyx_t_4 == (PY_LONG_LONG)-1) && PyErr_Occurred())) __PYX_ERR(0, 591, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyInt_As_PY_LONG_LONG(__pyx_t_2); if (unlikely((__pyx_t_4 == (PY_LONG_LONG)-1) && PyErr_Occurred())) __PYX_ERR(0, 606, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_PyInt_From_PY_LONG_LONG((1 + Storm::GetIndex::front_poisson(__pyx_t_4))); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 591, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_From_PY_LONG_LONG((1 + Storm::GetIndex::front_poisson(__pyx_t_4))); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 606, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_5 = NULL;
   __pyx_t_6 = 0;
   #if CYTHON_UNPACK_METHODS
   if (likely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_5)) {
@@ -15163,62 +15728,62 @@
   }
   #endif
   {
     PyObject *__pyx_callargs[2] = {__pyx_t_5, __pyx_t_2};
     __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_6, 1+__pyx_t_6);
     __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 591, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 606, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   }
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "Fortuna.pyx":592
+  /* "Fortuna.pyx":607
  *     def __call__(self, *args, **kwargs):
  *         self.data.rotate(1 + _front_poisson(self.rotate_size))
  *         return flatten(self.data[-1], *args, flat=self.flat, **kwargs)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_flatten); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 592, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_flatten); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 607, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_data); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 592, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_data); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 607, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_2 = __Pyx_GetItemInt(__pyx_t_3, -1L, long, 1, __Pyx_PyInt_From_long, 0, 1, 1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 592, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_GetItemInt(__pyx_t_3, -1L, long, 1, __Pyx_PyInt_From_long, 0, 1, 1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 607, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = PyTuple_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 592, __pyx_L1_error)
+  __pyx_t_3 = PyTuple_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 607, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_GIVEREF(__pyx_t_2);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_2)) __PYX_ERR(0, 592, __pyx_L1_error);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_2)) __PYX_ERR(0, 607, __pyx_L1_error);
   __pyx_t_2 = 0;
-  __pyx_t_2 = PyNumber_Add(__pyx_t_3, __pyx_v_args); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 592, __pyx_L1_error)
+  __pyx_t_2 = PyNumber_Add(__pyx_t_3, __pyx_v_args); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 607, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 592, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 607, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_flat); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 592, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_flat); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 607, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_flat, __pyx_t_7) < 0) __PYX_ERR(0, 592, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_flat, __pyx_t_7) < 0) __PYX_ERR(0, 607, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
   __pyx_t_3 = __pyx_t_5;
   __pyx_t_5 = 0;
-  if (__Pyx_MergeKeywords(__pyx_t_3, __pyx_v_kwargs) < 0) __PYX_ERR(0, 592, __pyx_L1_error)
-  __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_2, __pyx_t_3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 592, __pyx_L1_error)
+  if (__Pyx_MergeKeywords(__pyx_t_3, __pyx_v_kwargs) < 0) __PYX_ERR(0, 607, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_2, __pyx_t_3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 607, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_r = __pyx_t_5;
   __pyx_t_5 = 0;
   goto __pyx_L0;
 
-  /* "Fortuna.pyx":590
+  /* "Fortuna.pyx":605
  *         self.rotate_size = int(sqrt(len(self.data)))
  * 
  *     def __call__(self, *args, **kwargs):             # <<<<<<<<<<<<<<
  *         self.data.rotate(1 + _front_poisson(self.rotate_size))
  *         return flatten(self.data[-1], *args, flat=self.flat, **kwargs)
  */
 
@@ -15233,15 +15798,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "Fortuna.pyx":610
+/* "Fortuna.pyx":625
  *     __slots__ = ("flat", "size", "data", "truffle_shuffle", "cycles")
  * 
  *     def __init__(self, collection: Iterable, flat: bool = True):             # <<<<<<<<<<<<<<
  *         self.flat = flat
  *         self.data = tuple(collection)
  */
 
@@ -15302,37 +15867,37 @@
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_self)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 610, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 625, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_collection)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[1]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 610, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 625, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("__init__", 0, 2, 3, 1); __PYX_ERR(0, 610, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__init__", 0, 2, 3, 1); __PYX_ERR(0, 625, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (kw_args > 0) {
           PyObject* value = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_flat);
           if (value) { values[2] = __Pyx_Arg_NewRef_FASTCALL(value); kw_args--; }
-          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 610, __pyx_L3_error)
+          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 625, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "__init__") < 0)) __PYX_ERR(0, 610, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "__init__") < 0)) __PYX_ERR(0, 625, __pyx_L3_error)
       }
     } else {
       switch (__pyx_nargs) {
         case  3: values[2] = __Pyx_Arg_FASTCALL(__pyx_args, 2);
         CYTHON_FALLTHROUGH;
         case  2: values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
         values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
@@ -15342,15 +15907,15 @@
     }
     __pyx_v_self = values[0];
     __pyx_v_collection = values[1];
     __pyx_v_flat = values[2];
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__init__", 0, 2, 3, __pyx_nargs); __PYX_ERR(0, 610, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__init__", 0, 2, 3, __pyx_nargs); __PYX_ERR(0, 625, __pyx_L3_error)
   __pyx_L6_skip:;
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
@@ -15384,85 +15949,85 @@
   PyObject *__pyx_t_6 = NULL;
   int __pyx_t_7;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__init__", 1);
 
-  /* "Fortuna.pyx":611
+  /* "Fortuna.pyx":626
  * 
  *     def __init__(self, collection: Iterable, flat: bool = True):
  *         self.flat = flat             # <<<<<<<<<<<<<<
  *         self.data = tuple(collection)
  *         self.size = len(self.data)
  */
-  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_flat, __pyx_v_flat) < 0) __PYX_ERR(0, 611, __pyx_L1_error)
+  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_flat, __pyx_v_flat) < 0) __PYX_ERR(0, 626, __pyx_L1_error)
 
-  /* "Fortuna.pyx":612
+  /* "Fortuna.pyx":627
  *     def __init__(self, collection: Iterable, flat: bool = True):
  *         self.flat = flat
  *         self.data = tuple(collection)             # <<<<<<<<<<<<<<
  *         self.size = len(self.data)
  *         assert self.size > 0, "Input Error, Empty Container"
  */
-  __pyx_t_1 = __Pyx_PySequence_Tuple(__pyx_v_collection); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 612, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PySequence_Tuple(__pyx_v_collection); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 627, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_data, __pyx_t_1) < 0) __PYX_ERR(0, 612, __pyx_L1_error)
+  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_data, __pyx_t_1) < 0) __PYX_ERR(0, 627, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "Fortuna.pyx":613
+  /* "Fortuna.pyx":628
  *         self.flat = flat
  *         self.data = tuple(collection)
  *         self.size = len(self.data)             # <<<<<<<<<<<<<<
  *         assert self.size > 0, "Input Error, Empty Container"
  *         self.cycles = cycle(self.data)
  */
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_data); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 613, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_data); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 628, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = PyObject_Length(__pyx_t_1); if (unlikely(__pyx_t_2 == ((Py_ssize_t)-1))) __PYX_ERR(0, 613, __pyx_L1_error)
+  __pyx_t_2 = PyObject_Length(__pyx_t_1); if (unlikely(__pyx_t_2 == ((Py_ssize_t)-1))) __PYX_ERR(0, 628, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = PyInt_FromSsize_t(__pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 613, __pyx_L1_error)
+  __pyx_t_1 = PyInt_FromSsize_t(__pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 628, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_size, __pyx_t_1) < 0) __PYX_ERR(0, 613, __pyx_L1_error)
+  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_size, __pyx_t_1) < 0) __PYX_ERR(0, 628, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "Fortuna.pyx":614
+  /* "Fortuna.pyx":629
  *         self.data = tuple(collection)
  *         self.size = len(self.data)
  *         assert self.size > 0, "Input Error, Empty Container"             # <<<<<<<<<<<<<<
  *         self.cycles = cycle(self.data)
  *         self.truffle_shuffle = TruffleShuffle(self.data, flat)
  */
   #ifndef CYTHON_WITHOUT_ASSERTIONS
   if (unlikely(__pyx_assertions_enabled())) {
-    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_size); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 614, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_size); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 629, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_3 = PyObject_RichCompare(__pyx_t_1, __pyx_int_0, Py_GT); __Pyx_XGOTREF(__pyx_t_3); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 614, __pyx_L1_error)
+    __pyx_t_3 = PyObject_RichCompare(__pyx_t_1, __pyx_int_0, Py_GT); __Pyx_XGOTREF(__pyx_t_3); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 629, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __pyx_t_4 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely((__pyx_t_4 < 0))) __PYX_ERR(0, 614, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely((__pyx_t_4 < 0))) __PYX_ERR(0, 629, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     if (unlikely(!__pyx_t_4)) {
       __Pyx_Raise(__pyx_builtin_AssertionError, __pyx_kp_u_Input_Error_Empty_Container, 0, 0);
-      __PYX_ERR(0, 614, __pyx_L1_error)
+      __PYX_ERR(0, 629, __pyx_L1_error)
     }
   }
   #else
-  if ((1)); else __PYX_ERR(0, 614, __pyx_L1_error)
+  if ((1)); else __PYX_ERR(0, 629, __pyx_L1_error)
   #endif
 
-  /* "Fortuna.pyx":615
+  /* "Fortuna.pyx":630
  *         self.size = len(self.data)
  *         assert self.size > 0, "Input Error, Empty Container"
  *         self.cycles = cycle(self.data)             # <<<<<<<<<<<<<<
  *         self.truffle_shuffle = TruffleShuffle(self.data, flat)
  * 
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_cycle); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 615, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_cycle); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 630, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_data); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 615, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_data); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 630, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __pyx_t_6 = NULL;
   __pyx_t_7 = 0;
   #if CYTHON_UNPACK_METHODS
   if (unlikely(PyMethod_Check(__pyx_t_1))) {
     __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_1);
     if (likely(__pyx_t_6)) {
@@ -15475,31 +16040,31 @@
   }
   #endif
   {
     PyObject *__pyx_callargs[2] = {__pyx_t_6, __pyx_t_5};
     __pyx_t_3 = __Pyx_PyObject_FastCall(__pyx_t_1, __pyx_callargs+1-__pyx_t_7, 1+__pyx_t_7);
     __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-    if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 615, __pyx_L1_error)
+    if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 630, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   }
-  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_cycles, __pyx_t_3) < 0) __PYX_ERR(0, 615, __pyx_L1_error)
+  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_cycles, __pyx_t_3) < 0) __PYX_ERR(0, 630, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "Fortuna.pyx":616
+  /* "Fortuna.pyx":631
  *         assert self.size > 0, "Input Error, Empty Container"
  *         self.cycles = cycle(self.data)
  *         self.truffle_shuffle = TruffleShuffle(self.data, flat)             # <<<<<<<<<<<<<<
  * 
  *     def __call__(self, *args, **kwargs):
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_TruffleShuffle); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 616, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_TruffleShuffle); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 631, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_data); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 616, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_data); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 631, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __pyx_t_6 = NULL;
   __pyx_t_7 = 0;
   #if CYTHON_UNPACK_METHODS
   if (unlikely(PyMethod_Check(__pyx_t_1))) {
     __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_1);
     if (likely(__pyx_t_6)) {
@@ -15512,22 +16077,22 @@
   }
   #endif
   {
     PyObject *__pyx_callargs[3] = {__pyx_t_6, __pyx_t_5, __pyx_v_flat};
     __pyx_t_3 = __Pyx_PyObject_FastCall(__pyx_t_1, __pyx_callargs+1-__pyx_t_7, 2+__pyx_t_7);
     __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-    if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 616, __pyx_L1_error)
+    if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 631, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   }
-  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_truffle_shuffle, __pyx_t_3) < 0) __PYX_ERR(0, 616, __pyx_L1_error)
+  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_truffle_shuffle, __pyx_t_3) < 0) __PYX_ERR(0, 631, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "Fortuna.pyx":610
+  /* "Fortuna.pyx":625
  *     __slots__ = ("flat", "size", "data", "truffle_shuffle", "cycles")
  * 
  *     def __init__(self, collection: Iterable, flat: bool = True):             # <<<<<<<<<<<<<<
  *         self.flat = flat
  *         self.data = tuple(collection)
  */
 
@@ -15543,15 +16108,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "Fortuna.pyx":618
+/* "Fortuna.pyx":633
  *         self.truffle_shuffle = TruffleShuffle(self.data, flat)
  * 
  *     def __call__(self, *args, **kwargs):             # <<<<<<<<<<<<<<
  *         return self.quantum_monty(*args, **kwargs)
  * 
  */
 
@@ -15616,32 +16181,32 @@
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_self)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 618, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 633, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
         const Py_ssize_t used_pos_args = (kwd_pos_args < 1) ? kwd_pos_args : 1;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, __pyx_v_kwargs, values + 0, used_pos_args, "__call__") < 0)) __PYX_ERR(0, 618, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, __pyx_v_kwargs, values + 0, used_pos_args, "__call__") < 0)) __PYX_ERR(0, 633, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs < 1)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
     }
     __pyx_v_self = values[0];
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__call__", 0, 1, 1, __pyx_nargs); __PYX_ERR(0, 618, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__call__", 0, 1, 1, __pyx_nargs); __PYX_ERR(0, 633, __pyx_L3_error)
   __pyx_L6_skip:;
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
@@ -15675,35 +16240,35 @@
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__call__", 1);
 
-  /* "Fortuna.pyx":619
+  /* "Fortuna.pyx":634
  * 
  *     def __call__(self, *args, **kwargs):
  *         return self.quantum_monty(*args, **kwargs)             # <<<<<<<<<<<<<<
  * 
  *     def dispatch(self, monty: str) -> Callable:
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_quantum_monty); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 619, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_quantum_monty); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 634, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = PyDict_Copy(__pyx_v_kwargs); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 619, __pyx_L1_error)
+  __pyx_t_2 = PyDict_Copy(__pyx_v_kwargs); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 634, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_v_args, __pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 619, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_v_args, __pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 634, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_r = __pyx_t_3;
   __pyx_t_3 = 0;
   goto __pyx_L0;
 
-  /* "Fortuna.pyx":618
+  /* "Fortuna.pyx":633
  *         self.truffle_shuffle = TruffleShuffle(self.data, flat)
  * 
  *     def __call__(self, *args, **kwargs):             # <<<<<<<<<<<<<<
  *         return self.quantum_monty(*args, **kwargs)
  * 
  */
 
@@ -15716,15 +16281,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "Fortuna.pyx":621
+/* "Fortuna.pyx":636
  *         return self.quantum_monty(*args, **kwargs)
  * 
  *     def dispatch(self, monty: str) -> Callable:             # <<<<<<<<<<<<<<
  *         """ For dispatch automation.
  *         In general, prefer to use the methods directly when possible. """
  */
 
@@ -15781,57 +16346,57 @@
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_self)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 621, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 636, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_monty)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[1]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 621, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 636, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("dispatch", 1, 2, 2, 1); __PYX_ERR(0, 621, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("dispatch", 1, 2, 2, 1); __PYX_ERR(0, 636, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "dispatch") < 0)) __PYX_ERR(0, 621, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "dispatch") < 0)) __PYX_ERR(0, 636, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs != 2)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
       values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
     }
     __pyx_v_self = values[0];
     __pyx_v_monty = ((PyObject*)values[1]);
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("dispatch", 1, 2, 2, __pyx_nargs); __PYX_ERR(0, 621, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("dispatch", 1, 2, 2, __pyx_nargs); __PYX_ERR(0, 636, __pyx_L3_error)
   __pyx_L6_skip:;
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_AddTraceback("Fortuna.QuantumMonty.dispatch", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_monty), (&PyUnicode_Type), 0, "monty", 1))) __PYX_ERR(0, 621, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_monty), (&PyUnicode_Type), 0, "monty", 1))) __PYX_ERR(0, 636, __pyx_L1_error)
   __pyx_r = __pyx_pf_7Fortuna_12QuantumMonty_4dispatch(__pyx_self, __pyx_v_self, __pyx_v_monty);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
@@ -15851,232 +16416,232 @@
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("dispatch", 1);
 
-  /* "Fortuna.pyx":624
+  /* "Fortuna.pyx":639
  *         """ For dispatch automation.
  *         In general, prefer to use the methods directly when possible. """
  *         return {             # <<<<<<<<<<<<<<
  *             "flat_uniform": self.flat_uniform,
  *             "cycle": self.cycle,
  */
   __Pyx_XDECREF(__pyx_r);
 
-  /* "Fortuna.pyx":625
+  /* "Fortuna.pyx":640
  *         In general, prefer to use the methods directly when possible. """
  *         return {
  *             "flat_uniform": self.flat_uniform,             # <<<<<<<<<<<<<<
  *             "cycle": self.cycle,
  *             "truffle_shuffle": self.truffle_shuffle,
  */
-  __pyx_t_1 = __Pyx_PyDict_NewPresized(16); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 625, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyDict_NewPresized(16); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 640, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_flat_uniform); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 625, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_flat_uniform); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 640, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_flat_uniform, __pyx_t_2) < 0) __PYX_ERR(0, 625, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_flat_uniform, __pyx_t_2) < 0) __PYX_ERR(0, 640, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "Fortuna.pyx":626
+  /* "Fortuna.pyx":641
  *         return {
  *             "flat_uniform": self.flat_uniform,
  *             "cycle": self.cycle,             # <<<<<<<<<<<<<<
  *             "truffle_shuffle": self.truffle_shuffle,
  *             "front_linear": self.front_linear,
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_cycle); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 626, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_cycle); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 641, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_cycle, __pyx_t_2) < 0) __PYX_ERR(0, 625, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_cycle, __pyx_t_2) < 0) __PYX_ERR(0, 640, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "Fortuna.pyx":627
+  /* "Fortuna.pyx":642
  *             "flat_uniform": self.flat_uniform,
  *             "cycle": self.cycle,
  *             "truffle_shuffle": self.truffle_shuffle,             # <<<<<<<<<<<<<<
  *             "front_linear": self.front_linear,
  *             "middle_linear": self.middle_linear,
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_truffle_shuffle); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 627, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_truffle_shuffle); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 642, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_truffle_shuffle, __pyx_t_2) < 0) __PYX_ERR(0, 625, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_truffle_shuffle, __pyx_t_2) < 0) __PYX_ERR(0, 640, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "Fortuna.pyx":628
+  /* "Fortuna.pyx":643
  *             "cycle": self.cycle,
  *             "truffle_shuffle": self.truffle_shuffle,
  *             "front_linear": self.front_linear,             # <<<<<<<<<<<<<<
  *             "middle_linear": self.middle_linear,
  *             "back_linear": self.back_linear,
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_front_linear); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 628, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_front_linear); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 643, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_front_linear, __pyx_t_2) < 0) __PYX_ERR(0, 625, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_front_linear, __pyx_t_2) < 0) __PYX_ERR(0, 640, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "Fortuna.pyx":629
+  /* "Fortuna.pyx":644
  *             "truffle_shuffle": self.truffle_shuffle,
  *             "front_linear": self.front_linear,
  *             "middle_linear": self.middle_linear,             # <<<<<<<<<<<<<<
  *             "back_linear": self.back_linear,
  *             "quantum_linear": self.quantum_linear,
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_middle_linear); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 629, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_middle_linear); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 644, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_middle_linear, __pyx_t_2) < 0) __PYX_ERR(0, 625, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_middle_linear, __pyx_t_2) < 0) __PYX_ERR(0, 640, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "Fortuna.pyx":630
+  /* "Fortuna.pyx":645
  *             "front_linear": self.front_linear,
  *             "middle_linear": self.middle_linear,
  *             "back_linear": self.back_linear,             # <<<<<<<<<<<<<<
  *             "quantum_linear": self.quantum_linear,
  *             "front_gauss": self.front_gauss,
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_back_linear); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 630, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_back_linear); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 645, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_back_linear, __pyx_t_2) < 0) __PYX_ERR(0, 625, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_back_linear, __pyx_t_2) < 0) __PYX_ERR(0, 640, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "Fortuna.pyx":631
+  /* "Fortuna.pyx":646
  *             "middle_linear": self.middle_linear,
  *             "back_linear": self.back_linear,
  *             "quantum_linear": self.quantum_linear,             # <<<<<<<<<<<<<<
  *             "front_gauss": self.front_gauss,
  *             "middle_gauss": self.middle_gauss,
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_quantum_linear); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 631, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_quantum_linear); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 646, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_quantum_linear, __pyx_t_2) < 0) __PYX_ERR(0, 625, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_quantum_linear, __pyx_t_2) < 0) __PYX_ERR(0, 640, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "Fortuna.pyx":632
+  /* "Fortuna.pyx":647
  *             "back_linear": self.back_linear,
  *             "quantum_linear": self.quantum_linear,
  *             "front_gauss": self.front_gauss,             # <<<<<<<<<<<<<<
  *             "middle_gauss": self.middle_gauss,
  *             "back_gauss": self.back_gauss,
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_front_gauss); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 632, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_front_gauss); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 647, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_front_gauss, __pyx_t_2) < 0) __PYX_ERR(0, 625, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_front_gauss, __pyx_t_2) < 0) __PYX_ERR(0, 640, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "Fortuna.pyx":633
+  /* "Fortuna.pyx":648
  *             "quantum_linear": self.quantum_linear,
  *             "front_gauss": self.front_gauss,
  *             "middle_gauss": self.middle_gauss,             # <<<<<<<<<<<<<<
  *             "back_gauss": self.back_gauss,
  *             "quantum_gauss": self.quantum_gauss,
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_middle_gauss); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 633, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_middle_gauss); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 648, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_middle_gauss, __pyx_t_2) < 0) __PYX_ERR(0, 625, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_middle_gauss, __pyx_t_2) < 0) __PYX_ERR(0, 640, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "Fortuna.pyx":634
+  /* "Fortuna.pyx":649
  *             "front_gauss": self.front_gauss,
  *             "middle_gauss": self.middle_gauss,
  *             "back_gauss": self.back_gauss,             # <<<<<<<<<<<<<<
  *             "quantum_gauss": self.quantum_gauss,
  *             "front_poisson": self.front_poisson,
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_back_gauss); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 634, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_back_gauss); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 649, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_back_gauss, __pyx_t_2) < 0) __PYX_ERR(0, 625, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_back_gauss, __pyx_t_2) < 0) __PYX_ERR(0, 640, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "Fortuna.pyx":635
+  /* "Fortuna.pyx":650
  *             "middle_gauss": self.middle_gauss,
  *             "back_gauss": self.back_gauss,
  *             "quantum_gauss": self.quantum_gauss,             # <<<<<<<<<<<<<<
  *             "front_poisson": self.front_poisson,
  *             "middle_poisson": self.middle_poisson,
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_quantum_gauss); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 635, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_quantum_gauss); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 650, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_quantum_gauss, __pyx_t_2) < 0) __PYX_ERR(0, 625, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_quantum_gauss, __pyx_t_2) < 0) __PYX_ERR(0, 640, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "Fortuna.pyx":636
+  /* "Fortuna.pyx":651
  *             "back_gauss": self.back_gauss,
  *             "quantum_gauss": self.quantum_gauss,
  *             "front_poisson": self.front_poisson,             # <<<<<<<<<<<<<<
  *             "middle_poisson": self.middle_poisson,
  *             "back_poisson": self.back_poisson,
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_front_poisson); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 636, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_front_poisson); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 651, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_front_poisson, __pyx_t_2) < 0) __PYX_ERR(0, 625, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_front_poisson, __pyx_t_2) < 0) __PYX_ERR(0, 640, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "Fortuna.pyx":637
+  /* "Fortuna.pyx":652
  *             "quantum_gauss": self.quantum_gauss,
  *             "front_poisson": self.front_poisson,
  *             "middle_poisson": self.middle_poisson,             # <<<<<<<<<<<<<<
  *             "back_poisson": self.back_poisson,
  *             "quantum_poisson": self.quantum_poisson,
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_middle_poisson); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 637, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_middle_poisson); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 652, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_middle_poisson, __pyx_t_2) < 0) __PYX_ERR(0, 625, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_middle_poisson, __pyx_t_2) < 0) __PYX_ERR(0, 640, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "Fortuna.pyx":638
+  /* "Fortuna.pyx":653
  *             "front_poisson": self.front_poisson,
  *             "middle_poisson": self.middle_poisson,
  *             "back_poisson": self.back_poisson,             # <<<<<<<<<<<<<<
  *             "quantum_poisson": self.quantum_poisson,
  *             "quantum_monty": self.quantum_monty,
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_back_poisson); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 638, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_back_poisson); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 653, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_back_poisson, __pyx_t_2) < 0) __PYX_ERR(0, 625, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_back_poisson, __pyx_t_2) < 0) __PYX_ERR(0, 640, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "Fortuna.pyx":639
+  /* "Fortuna.pyx":654
  *             "middle_poisson": self.middle_poisson,
  *             "back_poisson": self.back_poisson,
  *             "quantum_poisson": self.quantum_poisson,             # <<<<<<<<<<<<<<
  *             "quantum_monty": self.quantum_monty,
  *         }[monty]
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_quantum_poisson); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 639, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_quantum_poisson); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 654, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_quantum_poisson, __pyx_t_2) < 0) __PYX_ERR(0, 625, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_quantum_poisson, __pyx_t_2) < 0) __PYX_ERR(0, 640, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "Fortuna.pyx":640
+  /* "Fortuna.pyx":655
  *             "back_poisson": self.back_poisson,
  *             "quantum_poisson": self.quantum_poisson,
  *             "quantum_monty": self.quantum_monty,             # <<<<<<<<<<<<<<
  *         }[monty]
  * 
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_quantum_monty); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 640, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_quantum_monty); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 655, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_quantum_monty, __pyx_t_2) < 0) __PYX_ERR(0, 625, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_quantum_monty, __pyx_t_2) < 0) __PYX_ERR(0, 640, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "Fortuna.pyx":641
+  /* "Fortuna.pyx":656
  *             "quantum_poisson": self.quantum_poisson,
  *             "quantum_monty": self.quantum_monty,
  *         }[monty]             # <<<<<<<<<<<<<<
  * 
  *     def flat_uniform(self, *args, **kwargs):
  */
-  __pyx_t_2 = __Pyx_PyDict_GetItem(__pyx_t_1, __pyx_v_monty); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 641, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyDict_GetItem(__pyx_t_1, __pyx_v_monty); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 656, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "Fortuna.pyx":621
+  /* "Fortuna.pyx":636
  *         return self.quantum_monty(*args, **kwargs)
  * 
  *     def dispatch(self, monty: str) -> Callable:             # <<<<<<<<<<<<<<
  *         """ For dispatch automation.
  *         In general, prefer to use the methods directly when possible. """
  */
 
@@ -16088,15 +16653,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "Fortuna.pyx":643
+/* "Fortuna.pyx":658
  *         }[monty]
  * 
  *     def flat_uniform(self, *args, **kwargs):             # <<<<<<<<<<<<<<
  *         return flatten(
  *             self.data[_random_index(self.size)], *args, flat=self.flat, **kwargs
  */
 
@@ -16161,32 +16726,32 @@
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_self)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 643, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 658, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
         const Py_ssize_t used_pos_args = (kwd_pos_args < 1) ? kwd_pos_args : 1;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, __pyx_v_kwargs, values + 0, used_pos_args, "flat_uniform") < 0)) __PYX_ERR(0, 643, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, __pyx_v_kwargs, values + 0, used_pos_args, "flat_uniform") < 0)) __PYX_ERR(0, 658, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs < 1)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
     }
     __pyx_v_self = values[0];
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("flat_uniform", 0, 1, 1, __pyx_nargs); __PYX_ERR(0, 643, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("flat_uniform", 0, 1, 1, __pyx_nargs); __PYX_ERR(0, 658, __pyx_L3_error)
   __pyx_L6_skip:;
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
@@ -16224,109 +16789,109 @@
   PyObject *__pyx_t_6 = NULL;
   PyObject *__pyx_t_7 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("flat_uniform", 1);
 
-  /* "Fortuna.pyx":644
+  /* "Fortuna.pyx":659
  * 
  *     def flat_uniform(self, *args, **kwargs):
  *         return flatten(             # <<<<<<<<<<<<<<
  *             self.data[_random_index(self.size)], *args, flat=self.flat, **kwargs
  *         )
  */
   __Pyx_XDECREF(__pyx_r);
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_flatten); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 644, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_flatten); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 659, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
 
-  /* "Fortuna.pyx":645
+  /* "Fortuna.pyx":660
  *     def flat_uniform(self, *args, **kwargs):
  *         return flatten(
  *             self.data[_random_index(self.size)], *args, flat=self.flat, **kwargs             # <<<<<<<<<<<<<<
  *         )
  * 
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_data); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 645, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_data); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 660, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_size); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 645, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_size); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 660, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = __Pyx_PyInt_As_PY_LONG_LONG(__pyx_t_3); if (unlikely((__pyx_t_4 == (PY_LONG_LONG)-1) && PyErr_Occurred())) __PYX_ERR(0, 645, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyInt_As_PY_LONG_LONG(__pyx_t_3); if (unlikely((__pyx_t_4 == (PY_LONG_LONG)-1) && PyErr_Occurred())) __PYX_ERR(0, 660, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_t_5 = Storm::GetIndex::random_index(__pyx_t_4);
-  __pyx_t_3 = __Pyx_GetItemInt(__pyx_t_2, __pyx_t_5, PY_LONG_LONG, 1, __Pyx_PyInt_From_PY_LONG_LONG, 0, 1, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 645, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_GetItemInt(__pyx_t_2, __pyx_t_5, PY_LONG_LONG, 1, __Pyx_PyInt_From_PY_LONG_LONG, 0, 1, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 660, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "Fortuna.pyx":644
+  /* "Fortuna.pyx":659
  * 
  *     def flat_uniform(self, *args, **kwargs):
  *         return flatten(             # <<<<<<<<<<<<<<
  *             self.data[_random_index(self.size)], *args, flat=self.flat, **kwargs
  *         )
  */
-  __pyx_t_2 = PyTuple_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 644, __pyx_L1_error)
+  __pyx_t_2 = PyTuple_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 659, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_GIVEREF(__pyx_t_3);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_t_3)) __PYX_ERR(0, 644, __pyx_L1_error);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_t_3)) __PYX_ERR(0, 659, __pyx_L1_error);
   __pyx_t_3 = 0;
 
-  /* "Fortuna.pyx":645
+  /* "Fortuna.pyx":660
  *     def flat_uniform(self, *args, **kwargs):
  *         return flatten(
  *             self.data[_random_index(self.size)], *args, flat=self.flat, **kwargs             # <<<<<<<<<<<<<<
  *         )
  * 
  */
-  __pyx_t_3 = PyNumber_Add(__pyx_t_2, __pyx_v_args); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 644, __pyx_L1_error)
+  __pyx_t_3 = PyNumber_Add(__pyx_t_2, __pyx_v_args); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 659, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "Fortuna.pyx":644
+  /* "Fortuna.pyx":659
  * 
  *     def flat_uniform(self, *args, **kwargs):
  *         return flatten(             # <<<<<<<<<<<<<<
  *             self.data[_random_index(self.size)], *args, flat=self.flat, **kwargs
  *         )
  */
-  __pyx_t_6 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 645, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 660, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
 
-  /* "Fortuna.pyx":645
+  /* "Fortuna.pyx":660
  *     def flat_uniform(self, *args, **kwargs):
  *         return flatten(
  *             self.data[_random_index(self.size)], *args, flat=self.flat, **kwargs             # <<<<<<<<<<<<<<
  *         )
  * 
  */
-  __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_flat); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 645, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_flat); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 660, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  if (PyDict_SetItem(__pyx_t_6, __pyx_n_s_flat, __pyx_t_7) < 0) __PYX_ERR(0, 645, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_6, __pyx_n_s_flat, __pyx_t_7) < 0) __PYX_ERR(0, 660, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
   __pyx_t_2 = __pyx_t_6;
   __pyx_t_6 = 0;
-  if (__Pyx_MergeKeywords(__pyx_t_2, __pyx_v_kwargs) < 0) __PYX_ERR(0, 645, __pyx_L1_error)
+  if (__Pyx_MergeKeywords(__pyx_t_2, __pyx_v_kwargs) < 0) __PYX_ERR(0, 660, __pyx_L1_error)
 
-  /* "Fortuna.pyx":644
+  /* "Fortuna.pyx":659
  * 
  *     def flat_uniform(self, *args, **kwargs):
  *         return flatten(             # <<<<<<<<<<<<<<
  *             self.data[_random_index(self.size)], *args, flat=self.flat, **kwargs
  *         )
  */
-  __pyx_t_6 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_3, __pyx_t_2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 644, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_3, __pyx_t_2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 659, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_r = __pyx_t_6;
   __pyx_t_6 = 0;
   goto __pyx_L0;
 
-  /* "Fortuna.pyx":643
+  /* "Fortuna.pyx":658
  *         }[monty]
  * 
  *     def flat_uniform(self, *args, **kwargs):             # <<<<<<<<<<<<<<
  *         return flatten(
  *             self.data[_random_index(self.size)], *args, flat=self.flat, **kwargs
  */
 
@@ -16341,15 +16906,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "Fortuna.pyx":648
+/* "Fortuna.pyx":663
  *         )
  * 
  *     def cycle(self, *args, **kwargs):             # <<<<<<<<<<<<<<
  *         return flatten(
  *             next(self.cycles), *args, flat=self.flat, **kwargs
  */
 
@@ -16414,32 +16979,32 @@
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_self)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 648, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 663, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
         const Py_ssize_t used_pos_args = (kwd_pos_args < 1) ? kwd_pos_args : 1;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, __pyx_v_kwargs, values + 0, used_pos_args, "cycle") < 0)) __PYX_ERR(0, 648, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, __pyx_v_kwargs, values + 0, used_pos_args, "cycle") < 0)) __PYX_ERR(0, 663, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs < 1)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
     }
     __pyx_v_self = values[0];
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("cycle", 0, 1, 1, __pyx_nargs); __PYX_ERR(0, 648, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("cycle", 0, 1, 1, __pyx_nargs); __PYX_ERR(0, 663, __pyx_L3_error)
   __pyx_L6_skip:;
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
@@ -16475,104 +17040,104 @@
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("cycle", 1);
 
-  /* "Fortuna.pyx":649
+  /* "Fortuna.pyx":664
  * 
  *     def cycle(self, *args, **kwargs):
  *         return flatten(             # <<<<<<<<<<<<<<
  *             next(self.cycles), *args, flat=self.flat, **kwargs
  *         )
  */
   __Pyx_XDECREF(__pyx_r);
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_flatten); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 649, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_flatten); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 664, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
 
-  /* "Fortuna.pyx":650
+  /* "Fortuna.pyx":665
  *     def cycle(self, *args, **kwargs):
  *         return flatten(
  *             next(self.cycles), *args, flat=self.flat, **kwargs             # <<<<<<<<<<<<<<
  *         )
  * 
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_cycles); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 650, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_cycles); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 665, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyIter_Next(__pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 650, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyIter_Next(__pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 665, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "Fortuna.pyx":649
+  /* "Fortuna.pyx":664
  * 
  *     def cycle(self, *args, **kwargs):
  *         return flatten(             # <<<<<<<<<<<<<<
  *             next(self.cycles), *args, flat=self.flat, **kwargs
  *         )
  */
-  __pyx_t_2 = PyTuple_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 649, __pyx_L1_error)
+  __pyx_t_2 = PyTuple_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 664, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_GIVEREF(__pyx_t_3);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_t_3)) __PYX_ERR(0, 649, __pyx_L1_error);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_t_3)) __PYX_ERR(0, 664, __pyx_L1_error);
   __pyx_t_3 = 0;
 
-  /* "Fortuna.pyx":650
+  /* "Fortuna.pyx":665
  *     def cycle(self, *args, **kwargs):
  *         return flatten(
  *             next(self.cycles), *args, flat=self.flat, **kwargs             # <<<<<<<<<<<<<<
  *         )
  * 
  */
-  __pyx_t_3 = PyNumber_Add(__pyx_t_2, __pyx_v_args); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 649, __pyx_L1_error)
+  __pyx_t_3 = PyNumber_Add(__pyx_t_2, __pyx_v_args); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 664, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "Fortuna.pyx":649
+  /* "Fortuna.pyx":664
  * 
  *     def cycle(self, *args, **kwargs):
  *         return flatten(             # <<<<<<<<<<<<<<
  *             next(self.cycles), *args, flat=self.flat, **kwargs
  *         )
  */
-  __pyx_t_4 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 650, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 665, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
 
-  /* "Fortuna.pyx":650
+  /* "Fortuna.pyx":665
  *     def cycle(self, *args, **kwargs):
  *         return flatten(
  *             next(self.cycles), *args, flat=self.flat, **kwargs             # <<<<<<<<<<<<<<
  *         )
  * 
  */
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_flat); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 650, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_flat); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 665, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_flat, __pyx_t_5) < 0) __PYX_ERR(0, 650, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_flat, __pyx_t_5) < 0) __PYX_ERR(0, 665, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __pyx_t_2 = __pyx_t_4;
   __pyx_t_4 = 0;
-  if (__Pyx_MergeKeywords(__pyx_t_2, __pyx_v_kwargs) < 0) __PYX_ERR(0, 650, __pyx_L1_error)
+  if (__Pyx_MergeKeywords(__pyx_t_2, __pyx_v_kwargs) < 0) __PYX_ERR(0, 665, __pyx_L1_error)
 
-  /* "Fortuna.pyx":649
+  /* "Fortuna.pyx":664
  * 
  *     def cycle(self, *args, **kwargs):
  *         return flatten(             # <<<<<<<<<<<<<<
  *             next(self.cycles), *args, flat=self.flat, **kwargs
  *         )
  */
-  __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_3, __pyx_t_2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 649, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_3, __pyx_t_2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 664, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_r = __pyx_t_4;
   __pyx_t_4 = 0;
   goto __pyx_L0;
 
-  /* "Fortuna.pyx":648
+  /* "Fortuna.pyx":663
  *         )
  * 
  *     def cycle(self, *args, **kwargs):             # <<<<<<<<<<<<<<
  *         return flatten(
  *             next(self.cycles), *args, flat=self.flat, **kwargs
  */
 
@@ -16587,15 +17152,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "Fortuna.pyx":653
+/* "Fortuna.pyx":668
  *         )
  * 
  *     def front_linear(self, *args, **kwargs):             # <<<<<<<<<<<<<<
  *         return flatten(
  *             self.data[_front_linear(self.size)], *args, flat=self.flat, **kwargs
  */
 
@@ -16660,32 +17225,32 @@
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_self)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 653, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 668, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
         const Py_ssize_t used_pos_args = (kwd_pos_args < 1) ? kwd_pos_args : 1;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, __pyx_v_kwargs, values + 0, used_pos_args, "front_linear") < 0)) __PYX_ERR(0, 653, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, __pyx_v_kwargs, values + 0, used_pos_args, "front_linear") < 0)) __PYX_ERR(0, 668, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs < 1)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
     }
     __pyx_v_self = values[0];
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("front_linear", 0, 1, 1, __pyx_nargs); __PYX_ERR(0, 653, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("front_linear", 0, 1, 1, __pyx_nargs); __PYX_ERR(0, 668, __pyx_L3_error)
   __pyx_L6_skip:;
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
@@ -16723,109 +17288,109 @@
   PyObject *__pyx_t_6 = NULL;
   PyObject *__pyx_t_7 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("front_linear", 1);
 
-  /* "Fortuna.pyx":654
+  /* "Fortuna.pyx":669
  * 
  *     def front_linear(self, *args, **kwargs):
  *         return flatten(             # <<<<<<<<<<<<<<
  *             self.data[_front_linear(self.size)], *args, flat=self.flat, **kwargs
  *         )
  */
   __Pyx_XDECREF(__pyx_r);
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_flatten); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 654, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_flatten); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 669, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
 
-  /* "Fortuna.pyx":655
+  /* "Fortuna.pyx":670
  *     def front_linear(self, *args, **kwargs):
  *         return flatten(
  *             self.data[_front_linear(self.size)], *args, flat=self.flat, **kwargs             # <<<<<<<<<<<<<<
  *         )
  * 
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_data); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 655, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_data); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 670, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_size); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 655, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_size); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 670, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = __Pyx_PyInt_As_PY_LONG_LONG(__pyx_t_3); if (unlikely((__pyx_t_4 == (PY_LONG_LONG)-1) && PyErr_Occurred())) __PYX_ERR(0, 655, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyInt_As_PY_LONG_LONG(__pyx_t_3); if (unlikely((__pyx_t_4 == (PY_LONG_LONG)-1) && PyErr_Occurred())) __PYX_ERR(0, 670, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_t_5 = Storm::GetIndex::front_linear(__pyx_t_4);
-  __pyx_t_3 = __Pyx_GetItemInt(__pyx_t_2, __pyx_t_5, PY_LONG_LONG, 1, __Pyx_PyInt_From_PY_LONG_LONG, 0, 1, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 655, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_GetItemInt(__pyx_t_2, __pyx_t_5, PY_LONG_LONG, 1, __Pyx_PyInt_From_PY_LONG_LONG, 0, 1, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 670, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "Fortuna.pyx":654
+  /* "Fortuna.pyx":669
  * 
  *     def front_linear(self, *args, **kwargs):
  *         return flatten(             # <<<<<<<<<<<<<<
  *             self.data[_front_linear(self.size)], *args, flat=self.flat, **kwargs
  *         )
  */
-  __pyx_t_2 = PyTuple_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 654, __pyx_L1_error)
+  __pyx_t_2 = PyTuple_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 669, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_GIVEREF(__pyx_t_3);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_t_3)) __PYX_ERR(0, 654, __pyx_L1_error);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_t_3)) __PYX_ERR(0, 669, __pyx_L1_error);
   __pyx_t_3 = 0;
 
-  /* "Fortuna.pyx":655
+  /* "Fortuna.pyx":670
  *     def front_linear(self, *args, **kwargs):
  *         return flatten(
  *             self.data[_front_linear(self.size)], *args, flat=self.flat, **kwargs             # <<<<<<<<<<<<<<
  *         )
  * 
  */
-  __pyx_t_3 = PyNumber_Add(__pyx_t_2, __pyx_v_args); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 654, __pyx_L1_error)
+  __pyx_t_3 = PyNumber_Add(__pyx_t_2, __pyx_v_args); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 669, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "Fortuna.pyx":654
+  /* "Fortuna.pyx":669
  * 
  *     def front_linear(self, *args, **kwargs):
  *         return flatten(             # <<<<<<<<<<<<<<
  *             self.data[_front_linear(self.size)], *args, flat=self.flat, **kwargs
  *         )
  */
-  __pyx_t_6 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 655, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 670, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
 
-  /* "Fortuna.pyx":655
+  /* "Fortuna.pyx":670
  *     def front_linear(self, *args, **kwargs):
  *         return flatten(
  *             self.data[_front_linear(self.size)], *args, flat=self.flat, **kwargs             # <<<<<<<<<<<<<<
  *         )
  * 
  */
-  __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_flat); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 655, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_flat); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 670, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  if (PyDict_SetItem(__pyx_t_6, __pyx_n_s_flat, __pyx_t_7) < 0) __PYX_ERR(0, 655, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_6, __pyx_n_s_flat, __pyx_t_7) < 0) __PYX_ERR(0, 670, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
   __pyx_t_2 = __pyx_t_6;
   __pyx_t_6 = 0;
-  if (__Pyx_MergeKeywords(__pyx_t_2, __pyx_v_kwargs) < 0) __PYX_ERR(0, 655, __pyx_L1_error)
+  if (__Pyx_MergeKeywords(__pyx_t_2, __pyx_v_kwargs) < 0) __PYX_ERR(0, 670, __pyx_L1_error)
 
-  /* "Fortuna.pyx":654
+  /* "Fortuna.pyx":669
  * 
  *     def front_linear(self, *args, **kwargs):
  *         return flatten(             # <<<<<<<<<<<<<<
  *             self.data[_front_linear(self.size)], *args, flat=self.flat, **kwargs
  *         )
  */
-  __pyx_t_6 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_3, __pyx_t_2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 654, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_3, __pyx_t_2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 669, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_r = __pyx_t_6;
   __pyx_t_6 = 0;
   goto __pyx_L0;
 
-  /* "Fortuna.pyx":653
+  /* "Fortuna.pyx":668
  *         )
  * 
  *     def front_linear(self, *args, **kwargs):             # <<<<<<<<<<<<<<
  *         return flatten(
  *             self.data[_front_linear(self.size)], *args, flat=self.flat, **kwargs
  */
 
@@ -16840,15 +17405,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "Fortuna.pyx":658
+/* "Fortuna.pyx":673
  *         )
  * 
  *     def middle_linear(self, *args, **kwargs):             # <<<<<<<<<<<<<<
  *         return flatten(
  *             self.data[_middle_linear(self.size)], *args, flat=self.flat, **kwargs
  */
 
@@ -16913,32 +17478,32 @@
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_self)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 658, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 673, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
         const Py_ssize_t used_pos_args = (kwd_pos_args < 1) ? kwd_pos_args : 1;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, __pyx_v_kwargs, values + 0, used_pos_args, "middle_linear") < 0)) __PYX_ERR(0, 658, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, __pyx_v_kwargs, values + 0, used_pos_args, "middle_linear") < 0)) __PYX_ERR(0, 673, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs < 1)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
     }
     __pyx_v_self = values[0];
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("middle_linear", 0, 1, 1, __pyx_nargs); __PYX_ERR(0, 658, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("middle_linear", 0, 1, 1, __pyx_nargs); __PYX_ERR(0, 673, __pyx_L3_error)
   __pyx_L6_skip:;
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
@@ -16976,109 +17541,109 @@
   PyObject *__pyx_t_6 = NULL;
   PyObject *__pyx_t_7 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("middle_linear", 1);
 
-  /* "Fortuna.pyx":659
+  /* "Fortuna.pyx":674
  * 
  *     def middle_linear(self, *args, **kwargs):
  *         return flatten(             # <<<<<<<<<<<<<<
  *             self.data[_middle_linear(self.size)], *args, flat=self.flat, **kwargs
  *         )
  */
   __Pyx_XDECREF(__pyx_r);
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_flatten); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 659, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_flatten); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 674, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
 
-  /* "Fortuna.pyx":660
+  /* "Fortuna.pyx":675
  *     def middle_linear(self, *args, **kwargs):
  *         return flatten(
  *             self.data[_middle_linear(self.size)], *args, flat=self.flat, **kwargs             # <<<<<<<<<<<<<<
  *         )
  * 
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_data); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 660, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_data); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 675, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_size); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 660, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_size); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 675, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = __Pyx_PyInt_As_PY_LONG_LONG(__pyx_t_3); if (unlikely((__pyx_t_4 == (PY_LONG_LONG)-1) && PyErr_Occurred())) __PYX_ERR(0, 660, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyInt_As_PY_LONG_LONG(__pyx_t_3); if (unlikely((__pyx_t_4 == (PY_LONG_LONG)-1) && PyErr_Occurred())) __PYX_ERR(0, 675, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_t_5 = Storm::GetIndex::middle_linear(__pyx_t_4);
-  __pyx_t_3 = __Pyx_GetItemInt(__pyx_t_2, __pyx_t_5, PY_LONG_LONG, 1, __Pyx_PyInt_From_PY_LONG_LONG, 0, 1, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 660, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_GetItemInt(__pyx_t_2, __pyx_t_5, PY_LONG_LONG, 1, __Pyx_PyInt_From_PY_LONG_LONG, 0, 1, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 675, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "Fortuna.pyx":659
+  /* "Fortuna.pyx":674
  * 
  *     def middle_linear(self, *args, **kwargs):
  *         return flatten(             # <<<<<<<<<<<<<<
  *             self.data[_middle_linear(self.size)], *args, flat=self.flat, **kwargs
  *         )
  */
-  __pyx_t_2 = PyTuple_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 659, __pyx_L1_error)
+  __pyx_t_2 = PyTuple_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 674, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_GIVEREF(__pyx_t_3);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_t_3)) __PYX_ERR(0, 659, __pyx_L1_error);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_t_3)) __PYX_ERR(0, 674, __pyx_L1_error);
   __pyx_t_3 = 0;
 
-  /* "Fortuna.pyx":660
+  /* "Fortuna.pyx":675
  *     def middle_linear(self, *args, **kwargs):
  *         return flatten(
  *             self.data[_middle_linear(self.size)], *args, flat=self.flat, **kwargs             # <<<<<<<<<<<<<<
  *         )
  * 
  */
-  __pyx_t_3 = PyNumber_Add(__pyx_t_2, __pyx_v_args); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 659, __pyx_L1_error)
+  __pyx_t_3 = PyNumber_Add(__pyx_t_2, __pyx_v_args); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 674, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "Fortuna.pyx":659
+  /* "Fortuna.pyx":674
  * 
  *     def middle_linear(self, *args, **kwargs):
  *         return flatten(             # <<<<<<<<<<<<<<
  *             self.data[_middle_linear(self.size)], *args, flat=self.flat, **kwargs
  *         )
  */
-  __pyx_t_6 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 660, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 675, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
 
-  /* "Fortuna.pyx":660
+  /* "Fortuna.pyx":675
  *     def middle_linear(self, *args, **kwargs):
  *         return flatten(
  *             self.data[_middle_linear(self.size)], *args, flat=self.flat, **kwargs             # <<<<<<<<<<<<<<
  *         )
  * 
  */
-  __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_flat); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 660, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_flat); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 675, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  if (PyDict_SetItem(__pyx_t_6, __pyx_n_s_flat, __pyx_t_7) < 0) __PYX_ERR(0, 660, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_6, __pyx_n_s_flat, __pyx_t_7) < 0) __PYX_ERR(0, 675, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
   __pyx_t_2 = __pyx_t_6;
   __pyx_t_6 = 0;
-  if (__Pyx_MergeKeywords(__pyx_t_2, __pyx_v_kwargs) < 0) __PYX_ERR(0, 660, __pyx_L1_error)
+  if (__Pyx_MergeKeywords(__pyx_t_2, __pyx_v_kwargs) < 0) __PYX_ERR(0, 675, __pyx_L1_error)
 
-  /* "Fortuna.pyx":659
+  /* "Fortuna.pyx":674
  * 
  *     def middle_linear(self, *args, **kwargs):
  *         return flatten(             # <<<<<<<<<<<<<<
  *             self.data[_middle_linear(self.size)], *args, flat=self.flat, **kwargs
  *         )
  */
-  __pyx_t_6 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_3, __pyx_t_2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 659, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_3, __pyx_t_2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 674, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_r = __pyx_t_6;
   __pyx_t_6 = 0;
   goto __pyx_L0;
 
-  /* "Fortuna.pyx":658
+  /* "Fortuna.pyx":673
  *         )
  * 
  *     def middle_linear(self, *args, **kwargs):             # <<<<<<<<<<<<<<
  *         return flatten(
  *             self.data[_middle_linear(self.size)], *args, flat=self.flat, **kwargs
  */
 
@@ -17093,15 +17658,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "Fortuna.pyx":663
+/* "Fortuna.pyx":678
  *         )
  * 
  *     def back_linear(self, *args, **kwargs):             # <<<<<<<<<<<<<<
  *         return flatten(
  *             self.data[_back_linear(self.size)], *args, flat=self.flat, **kwargs
  */
 
@@ -17166,32 +17731,32 @@
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_self)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 663, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 678, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
         const Py_ssize_t used_pos_args = (kwd_pos_args < 1) ? kwd_pos_args : 1;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, __pyx_v_kwargs, values + 0, used_pos_args, "back_linear") < 0)) __PYX_ERR(0, 663, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, __pyx_v_kwargs, values + 0, used_pos_args, "back_linear") < 0)) __PYX_ERR(0, 678, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs < 1)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
     }
     __pyx_v_self = values[0];
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("back_linear", 0, 1, 1, __pyx_nargs); __PYX_ERR(0, 663, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("back_linear", 0, 1, 1, __pyx_nargs); __PYX_ERR(0, 678, __pyx_L3_error)
   __pyx_L6_skip:;
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
@@ -17229,109 +17794,109 @@
   PyObject *__pyx_t_6 = NULL;
   PyObject *__pyx_t_7 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("back_linear", 1);
 
-  /* "Fortuna.pyx":664
+  /* "Fortuna.pyx":679
  * 
  *     def back_linear(self, *args, **kwargs):
  *         return flatten(             # <<<<<<<<<<<<<<
  *             self.data[_back_linear(self.size)], *args, flat=self.flat, **kwargs
  *         )
  */
   __Pyx_XDECREF(__pyx_r);
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_flatten); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 664, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_flatten); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 679, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
 
-  /* "Fortuna.pyx":665
+  /* "Fortuna.pyx":680
  *     def back_linear(self, *args, **kwargs):
  *         return flatten(
  *             self.data[_back_linear(self.size)], *args, flat=self.flat, **kwargs             # <<<<<<<<<<<<<<
  *         )
  * 
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_data); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 665, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_data); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 680, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_size); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 665, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_size); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 680, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = __Pyx_PyInt_As_PY_LONG_LONG(__pyx_t_3); if (unlikely((__pyx_t_4 == (PY_LONG_LONG)-1) && PyErr_Occurred())) __PYX_ERR(0, 665, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyInt_As_PY_LONG_LONG(__pyx_t_3); if (unlikely((__pyx_t_4 == (PY_LONG_LONG)-1) && PyErr_Occurred())) __PYX_ERR(0, 680, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_t_5 = Storm::GetIndex::back_linear(__pyx_t_4);
-  __pyx_t_3 = __Pyx_GetItemInt(__pyx_t_2, __pyx_t_5, PY_LONG_LONG, 1, __Pyx_PyInt_From_PY_LONG_LONG, 0, 1, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 665, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_GetItemInt(__pyx_t_2, __pyx_t_5, PY_LONG_LONG, 1, __Pyx_PyInt_From_PY_LONG_LONG, 0, 1, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 680, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "Fortuna.pyx":664
+  /* "Fortuna.pyx":679
  * 
  *     def back_linear(self, *args, **kwargs):
  *         return flatten(             # <<<<<<<<<<<<<<
  *             self.data[_back_linear(self.size)], *args, flat=self.flat, **kwargs
  *         )
  */
-  __pyx_t_2 = PyTuple_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 664, __pyx_L1_error)
+  __pyx_t_2 = PyTuple_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 679, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_GIVEREF(__pyx_t_3);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_t_3)) __PYX_ERR(0, 664, __pyx_L1_error);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_t_3)) __PYX_ERR(0, 679, __pyx_L1_error);
   __pyx_t_3 = 0;
 
-  /* "Fortuna.pyx":665
+  /* "Fortuna.pyx":680
  *     def back_linear(self, *args, **kwargs):
  *         return flatten(
  *             self.data[_back_linear(self.size)], *args, flat=self.flat, **kwargs             # <<<<<<<<<<<<<<
  *         )
  * 
  */
-  __pyx_t_3 = PyNumber_Add(__pyx_t_2, __pyx_v_args); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 664, __pyx_L1_error)
+  __pyx_t_3 = PyNumber_Add(__pyx_t_2, __pyx_v_args); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 679, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "Fortuna.pyx":664
+  /* "Fortuna.pyx":679
  * 
  *     def back_linear(self, *args, **kwargs):
  *         return flatten(             # <<<<<<<<<<<<<<
  *             self.data[_back_linear(self.size)], *args, flat=self.flat, **kwargs
  *         )
  */
-  __pyx_t_6 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 665, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 680, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
 
-  /* "Fortuna.pyx":665
+  /* "Fortuna.pyx":680
  *     def back_linear(self, *args, **kwargs):
  *         return flatten(
  *             self.data[_back_linear(self.size)], *args, flat=self.flat, **kwargs             # <<<<<<<<<<<<<<
  *         )
  * 
  */
-  __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_flat); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 665, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_flat); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 680, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  if (PyDict_SetItem(__pyx_t_6, __pyx_n_s_flat, __pyx_t_7) < 0) __PYX_ERR(0, 665, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_6, __pyx_n_s_flat, __pyx_t_7) < 0) __PYX_ERR(0, 680, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
   __pyx_t_2 = __pyx_t_6;
   __pyx_t_6 = 0;
-  if (__Pyx_MergeKeywords(__pyx_t_2, __pyx_v_kwargs) < 0) __PYX_ERR(0, 665, __pyx_L1_error)
+  if (__Pyx_MergeKeywords(__pyx_t_2, __pyx_v_kwargs) < 0) __PYX_ERR(0, 680, __pyx_L1_error)
 
-  /* "Fortuna.pyx":664
+  /* "Fortuna.pyx":679
  * 
  *     def back_linear(self, *args, **kwargs):
  *         return flatten(             # <<<<<<<<<<<<<<
  *             self.data[_back_linear(self.size)], *args, flat=self.flat, **kwargs
  *         )
  */
-  __pyx_t_6 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_3, __pyx_t_2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 664, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_3, __pyx_t_2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 679, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_r = __pyx_t_6;
   __pyx_t_6 = 0;
   goto __pyx_L0;
 
-  /* "Fortuna.pyx":663
+  /* "Fortuna.pyx":678
  *         )
  * 
  *     def back_linear(self, *args, **kwargs):             # <<<<<<<<<<<<<<
  *         return flatten(
  *             self.data[_back_linear(self.size)], *args, flat=self.flat, **kwargs
  */
 
@@ -17346,15 +17911,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "Fortuna.pyx":668
+/* "Fortuna.pyx":683
  *         )
  * 
  *     def quantum_linear(self, *args, **kwargs):             # <<<<<<<<<<<<<<
  *         return flatten(
  *             self.data[_quantum_linear(self.size)], *args, flat=self.flat, **kwargs
  */
 
@@ -17419,32 +17984,32 @@
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_self)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 668, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 683, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
         const Py_ssize_t used_pos_args = (kwd_pos_args < 1) ? kwd_pos_args : 1;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, __pyx_v_kwargs, values + 0, used_pos_args, "quantum_linear") < 0)) __PYX_ERR(0, 668, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, __pyx_v_kwargs, values + 0, used_pos_args, "quantum_linear") < 0)) __PYX_ERR(0, 683, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs < 1)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
     }
     __pyx_v_self = values[0];
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("quantum_linear", 0, 1, 1, __pyx_nargs); __PYX_ERR(0, 668, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("quantum_linear", 0, 1, 1, __pyx_nargs); __PYX_ERR(0, 683, __pyx_L3_error)
   __pyx_L6_skip:;
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
@@ -17482,109 +18047,109 @@
   PyObject *__pyx_t_6 = NULL;
   PyObject *__pyx_t_7 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("quantum_linear", 1);
 
-  /* "Fortuna.pyx":669
+  /* "Fortuna.pyx":684
  * 
  *     def quantum_linear(self, *args, **kwargs):
  *         return flatten(             # <<<<<<<<<<<<<<
  *             self.data[_quantum_linear(self.size)], *args, flat=self.flat, **kwargs
  *         )
  */
   __Pyx_XDECREF(__pyx_r);
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_flatten); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 669, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_flatten); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 684, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
 
-  /* "Fortuna.pyx":670
+  /* "Fortuna.pyx":685
  *     def quantum_linear(self, *args, **kwargs):
  *         return flatten(
  *             self.data[_quantum_linear(self.size)], *args, flat=self.flat, **kwargs             # <<<<<<<<<<<<<<
  *         )
  * 
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_data); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 670, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_data); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 685, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_size); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 670, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_size); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 685, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = __Pyx_PyInt_As_PY_LONG_LONG(__pyx_t_3); if (unlikely((__pyx_t_4 == (PY_LONG_LONG)-1) && PyErr_Occurred())) __PYX_ERR(0, 670, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyInt_As_PY_LONG_LONG(__pyx_t_3); if (unlikely((__pyx_t_4 == (PY_LONG_LONG)-1) && PyErr_Occurred())) __PYX_ERR(0, 685, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_t_5 = Storm::GetIndex::quantum_linear(__pyx_t_4);
-  __pyx_t_3 = __Pyx_GetItemInt(__pyx_t_2, __pyx_t_5, PY_LONG_LONG, 1, __Pyx_PyInt_From_PY_LONG_LONG, 0, 1, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 670, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_GetItemInt(__pyx_t_2, __pyx_t_5, PY_LONG_LONG, 1, __Pyx_PyInt_From_PY_LONG_LONG, 0, 1, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 685, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "Fortuna.pyx":669
+  /* "Fortuna.pyx":684
  * 
  *     def quantum_linear(self, *args, **kwargs):
  *         return flatten(             # <<<<<<<<<<<<<<
  *             self.data[_quantum_linear(self.size)], *args, flat=self.flat, **kwargs
  *         )
  */
-  __pyx_t_2 = PyTuple_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 669, __pyx_L1_error)
+  __pyx_t_2 = PyTuple_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 684, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_GIVEREF(__pyx_t_3);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_t_3)) __PYX_ERR(0, 669, __pyx_L1_error);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_t_3)) __PYX_ERR(0, 684, __pyx_L1_error);
   __pyx_t_3 = 0;
 
-  /* "Fortuna.pyx":670
+  /* "Fortuna.pyx":685
  *     def quantum_linear(self, *args, **kwargs):
  *         return flatten(
  *             self.data[_quantum_linear(self.size)], *args, flat=self.flat, **kwargs             # <<<<<<<<<<<<<<
  *         )
  * 
  */
-  __pyx_t_3 = PyNumber_Add(__pyx_t_2, __pyx_v_args); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 669, __pyx_L1_error)
+  __pyx_t_3 = PyNumber_Add(__pyx_t_2, __pyx_v_args); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 684, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "Fortuna.pyx":669
+  /* "Fortuna.pyx":684
  * 
  *     def quantum_linear(self, *args, **kwargs):
  *         return flatten(             # <<<<<<<<<<<<<<
  *             self.data[_quantum_linear(self.size)], *args, flat=self.flat, **kwargs
  *         )
  */
-  __pyx_t_6 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 670, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 685, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
 
-  /* "Fortuna.pyx":670
+  /* "Fortuna.pyx":685
  *     def quantum_linear(self, *args, **kwargs):
  *         return flatten(
  *             self.data[_quantum_linear(self.size)], *args, flat=self.flat, **kwargs             # <<<<<<<<<<<<<<
  *         )
  * 
  */
-  __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_flat); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 670, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_flat); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 685, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  if (PyDict_SetItem(__pyx_t_6, __pyx_n_s_flat, __pyx_t_7) < 0) __PYX_ERR(0, 670, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_6, __pyx_n_s_flat, __pyx_t_7) < 0) __PYX_ERR(0, 685, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
   __pyx_t_2 = __pyx_t_6;
   __pyx_t_6 = 0;
-  if (__Pyx_MergeKeywords(__pyx_t_2, __pyx_v_kwargs) < 0) __PYX_ERR(0, 670, __pyx_L1_error)
+  if (__Pyx_MergeKeywords(__pyx_t_2, __pyx_v_kwargs) < 0) __PYX_ERR(0, 685, __pyx_L1_error)
 
-  /* "Fortuna.pyx":669
+  /* "Fortuna.pyx":684
  * 
  *     def quantum_linear(self, *args, **kwargs):
  *         return flatten(             # <<<<<<<<<<<<<<
  *             self.data[_quantum_linear(self.size)], *args, flat=self.flat, **kwargs
  *         )
  */
-  __pyx_t_6 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_3, __pyx_t_2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 669, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_3, __pyx_t_2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 684, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_r = __pyx_t_6;
   __pyx_t_6 = 0;
   goto __pyx_L0;
 
-  /* "Fortuna.pyx":668
+  /* "Fortuna.pyx":683
  *         )
  * 
  *     def quantum_linear(self, *args, **kwargs):             # <<<<<<<<<<<<<<
  *         return flatten(
  *             self.data[_quantum_linear(self.size)], *args, flat=self.flat, **kwargs
  */
 
@@ -17599,15 +18164,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "Fortuna.pyx":673
+/* "Fortuna.pyx":688
  *         )
  * 
  *     def front_gauss(self, *args, **kwargs):             # <<<<<<<<<<<<<<
  *         return flatten(
  *             self.data[_front_gauss(self.size)], *args, flat=self.flat, **kwargs)
  */
 
@@ -17672,32 +18237,32 @@
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_self)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 673, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 688, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
         const Py_ssize_t used_pos_args = (kwd_pos_args < 1) ? kwd_pos_args : 1;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, __pyx_v_kwargs, values + 0, used_pos_args, "front_gauss") < 0)) __PYX_ERR(0, 673, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, __pyx_v_kwargs, values + 0, used_pos_args, "front_gauss") < 0)) __PYX_ERR(0, 688, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs < 1)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
     }
     __pyx_v_self = values[0];
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("front_gauss", 0, 1, 1, __pyx_nargs); __PYX_ERR(0, 673, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("front_gauss", 0, 1, 1, __pyx_nargs); __PYX_ERR(0, 688, __pyx_L3_error)
   __pyx_L6_skip:;
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
@@ -17735,109 +18300,109 @@
   PyObject *__pyx_t_6 = NULL;
   PyObject *__pyx_t_7 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("front_gauss", 1);
 
-  /* "Fortuna.pyx":674
+  /* "Fortuna.pyx":689
  * 
  *     def front_gauss(self, *args, **kwargs):
  *         return flatten(             # <<<<<<<<<<<<<<
  *             self.data[_front_gauss(self.size)], *args, flat=self.flat, **kwargs)
  * 
  */
   __Pyx_XDECREF(__pyx_r);
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_flatten); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 674, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_flatten); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 689, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
 
-  /* "Fortuna.pyx":675
+  /* "Fortuna.pyx":690
  *     def front_gauss(self, *args, **kwargs):
  *         return flatten(
  *             self.data[_front_gauss(self.size)], *args, flat=self.flat, **kwargs)             # <<<<<<<<<<<<<<
  * 
  *     def middle_gauss(self, *args, **kwargs):
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_data); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 675, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_data); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 690, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_size); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 675, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_size); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 690, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = __Pyx_PyInt_As_PY_LONG_LONG(__pyx_t_3); if (unlikely((__pyx_t_4 == (PY_LONG_LONG)-1) && PyErr_Occurred())) __PYX_ERR(0, 675, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyInt_As_PY_LONG_LONG(__pyx_t_3); if (unlikely((__pyx_t_4 == (PY_LONG_LONG)-1) && PyErr_Occurred())) __PYX_ERR(0, 690, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_t_5 = Storm::GetIndex::front_gauss(__pyx_t_4);
-  __pyx_t_3 = __Pyx_GetItemInt(__pyx_t_2, __pyx_t_5, PY_LONG_LONG, 1, __Pyx_PyInt_From_PY_LONG_LONG, 0, 1, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 675, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_GetItemInt(__pyx_t_2, __pyx_t_5, PY_LONG_LONG, 1, __Pyx_PyInt_From_PY_LONG_LONG, 0, 1, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 690, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "Fortuna.pyx":674
+  /* "Fortuna.pyx":689
  * 
  *     def front_gauss(self, *args, **kwargs):
  *         return flatten(             # <<<<<<<<<<<<<<
  *             self.data[_front_gauss(self.size)], *args, flat=self.flat, **kwargs)
  * 
  */
-  __pyx_t_2 = PyTuple_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 674, __pyx_L1_error)
+  __pyx_t_2 = PyTuple_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 689, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_GIVEREF(__pyx_t_3);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_t_3)) __PYX_ERR(0, 674, __pyx_L1_error);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_t_3)) __PYX_ERR(0, 689, __pyx_L1_error);
   __pyx_t_3 = 0;
 
-  /* "Fortuna.pyx":675
+  /* "Fortuna.pyx":690
  *     def front_gauss(self, *args, **kwargs):
  *         return flatten(
  *             self.data[_front_gauss(self.size)], *args, flat=self.flat, **kwargs)             # <<<<<<<<<<<<<<
  * 
  *     def middle_gauss(self, *args, **kwargs):
  */
-  __pyx_t_3 = PyNumber_Add(__pyx_t_2, __pyx_v_args); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 674, __pyx_L1_error)
+  __pyx_t_3 = PyNumber_Add(__pyx_t_2, __pyx_v_args); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 689, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "Fortuna.pyx":674
+  /* "Fortuna.pyx":689
  * 
  *     def front_gauss(self, *args, **kwargs):
  *         return flatten(             # <<<<<<<<<<<<<<
  *             self.data[_front_gauss(self.size)], *args, flat=self.flat, **kwargs)
  * 
  */
-  __pyx_t_6 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 675, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 690, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
 
-  /* "Fortuna.pyx":675
+  /* "Fortuna.pyx":690
  *     def front_gauss(self, *args, **kwargs):
  *         return flatten(
  *             self.data[_front_gauss(self.size)], *args, flat=self.flat, **kwargs)             # <<<<<<<<<<<<<<
  * 
  *     def middle_gauss(self, *args, **kwargs):
  */
-  __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_flat); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 675, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_flat); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 690, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  if (PyDict_SetItem(__pyx_t_6, __pyx_n_s_flat, __pyx_t_7) < 0) __PYX_ERR(0, 675, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_6, __pyx_n_s_flat, __pyx_t_7) < 0) __PYX_ERR(0, 690, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
   __pyx_t_2 = __pyx_t_6;
   __pyx_t_6 = 0;
-  if (__Pyx_MergeKeywords(__pyx_t_2, __pyx_v_kwargs) < 0) __PYX_ERR(0, 675, __pyx_L1_error)
+  if (__Pyx_MergeKeywords(__pyx_t_2, __pyx_v_kwargs) < 0) __PYX_ERR(0, 690, __pyx_L1_error)
 
-  /* "Fortuna.pyx":674
+  /* "Fortuna.pyx":689
  * 
  *     def front_gauss(self, *args, **kwargs):
  *         return flatten(             # <<<<<<<<<<<<<<
  *             self.data[_front_gauss(self.size)], *args, flat=self.flat, **kwargs)
  * 
  */
-  __pyx_t_6 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_3, __pyx_t_2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 674, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_3, __pyx_t_2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 689, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_r = __pyx_t_6;
   __pyx_t_6 = 0;
   goto __pyx_L0;
 
-  /* "Fortuna.pyx":673
+  /* "Fortuna.pyx":688
  *         )
  * 
  *     def front_gauss(self, *args, **kwargs):             # <<<<<<<<<<<<<<
  *         return flatten(
  *             self.data[_front_gauss(self.size)], *args, flat=self.flat, **kwargs)
  */
 
@@ -17852,15 +18417,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "Fortuna.pyx":677
+/* "Fortuna.pyx":692
  *             self.data[_front_gauss(self.size)], *args, flat=self.flat, **kwargs)
  * 
  *     def middle_gauss(self, *args, **kwargs):             # <<<<<<<<<<<<<<
  *         return flatten(
  *             self.data[_middle_gauss(self.size)], *args, flat=self.flat, **kwargs
  */
 
@@ -17925,32 +18490,32 @@
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_self)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 677, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 692, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
         const Py_ssize_t used_pos_args = (kwd_pos_args < 1) ? kwd_pos_args : 1;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, __pyx_v_kwargs, values + 0, used_pos_args, "middle_gauss") < 0)) __PYX_ERR(0, 677, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, __pyx_v_kwargs, values + 0, used_pos_args, "middle_gauss") < 0)) __PYX_ERR(0, 692, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs < 1)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
     }
     __pyx_v_self = values[0];
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("middle_gauss", 0, 1, 1, __pyx_nargs); __PYX_ERR(0, 677, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("middle_gauss", 0, 1, 1, __pyx_nargs); __PYX_ERR(0, 692, __pyx_L3_error)
   __pyx_L6_skip:;
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
@@ -17988,109 +18553,109 @@
   PyObject *__pyx_t_6 = NULL;
   PyObject *__pyx_t_7 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("middle_gauss", 1);
 
-  /* "Fortuna.pyx":678
+  /* "Fortuna.pyx":693
  * 
  *     def middle_gauss(self, *args, **kwargs):
  *         return flatten(             # <<<<<<<<<<<<<<
  *             self.data[_middle_gauss(self.size)], *args, flat=self.flat, **kwargs
  *         )
  */
   __Pyx_XDECREF(__pyx_r);
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_flatten); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 678, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_flatten); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 693, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
 
-  /* "Fortuna.pyx":679
+  /* "Fortuna.pyx":694
  *     def middle_gauss(self, *args, **kwargs):
  *         return flatten(
  *             self.data[_middle_gauss(self.size)], *args, flat=self.flat, **kwargs             # <<<<<<<<<<<<<<
  *         )
  * 
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_data); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 679, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_data); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 694, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_size); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 679, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_size); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 694, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = __Pyx_PyInt_As_PY_LONG_LONG(__pyx_t_3); if (unlikely((__pyx_t_4 == (PY_LONG_LONG)-1) && PyErr_Occurred())) __PYX_ERR(0, 679, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyInt_As_PY_LONG_LONG(__pyx_t_3); if (unlikely((__pyx_t_4 == (PY_LONG_LONG)-1) && PyErr_Occurred())) __PYX_ERR(0, 694, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_t_5 = Storm::GetIndex::middle_gauss(__pyx_t_4);
-  __pyx_t_3 = __Pyx_GetItemInt(__pyx_t_2, __pyx_t_5, PY_LONG_LONG, 1, __Pyx_PyInt_From_PY_LONG_LONG, 0, 1, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 679, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_GetItemInt(__pyx_t_2, __pyx_t_5, PY_LONG_LONG, 1, __Pyx_PyInt_From_PY_LONG_LONG, 0, 1, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 694, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "Fortuna.pyx":678
+  /* "Fortuna.pyx":693
  * 
  *     def middle_gauss(self, *args, **kwargs):
  *         return flatten(             # <<<<<<<<<<<<<<
  *             self.data[_middle_gauss(self.size)], *args, flat=self.flat, **kwargs
  *         )
  */
-  __pyx_t_2 = PyTuple_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 678, __pyx_L1_error)
+  __pyx_t_2 = PyTuple_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 693, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_GIVEREF(__pyx_t_3);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_t_3)) __PYX_ERR(0, 678, __pyx_L1_error);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_t_3)) __PYX_ERR(0, 693, __pyx_L1_error);
   __pyx_t_3 = 0;
 
-  /* "Fortuna.pyx":679
+  /* "Fortuna.pyx":694
  *     def middle_gauss(self, *args, **kwargs):
  *         return flatten(
  *             self.data[_middle_gauss(self.size)], *args, flat=self.flat, **kwargs             # <<<<<<<<<<<<<<
  *         )
  * 
  */
-  __pyx_t_3 = PyNumber_Add(__pyx_t_2, __pyx_v_args); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 678, __pyx_L1_error)
+  __pyx_t_3 = PyNumber_Add(__pyx_t_2, __pyx_v_args); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 693, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "Fortuna.pyx":678
+  /* "Fortuna.pyx":693
  * 
  *     def middle_gauss(self, *args, **kwargs):
  *         return flatten(             # <<<<<<<<<<<<<<
  *             self.data[_middle_gauss(self.size)], *args, flat=self.flat, **kwargs
  *         )
  */
-  __pyx_t_6 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 679, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 694, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
 
-  /* "Fortuna.pyx":679
+  /* "Fortuna.pyx":694
  *     def middle_gauss(self, *args, **kwargs):
  *         return flatten(
  *             self.data[_middle_gauss(self.size)], *args, flat=self.flat, **kwargs             # <<<<<<<<<<<<<<
  *         )
  * 
  */
-  __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_flat); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 679, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_flat); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 694, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  if (PyDict_SetItem(__pyx_t_6, __pyx_n_s_flat, __pyx_t_7) < 0) __PYX_ERR(0, 679, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_6, __pyx_n_s_flat, __pyx_t_7) < 0) __PYX_ERR(0, 694, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
   __pyx_t_2 = __pyx_t_6;
   __pyx_t_6 = 0;
-  if (__Pyx_MergeKeywords(__pyx_t_2, __pyx_v_kwargs) < 0) __PYX_ERR(0, 679, __pyx_L1_error)
+  if (__Pyx_MergeKeywords(__pyx_t_2, __pyx_v_kwargs) < 0) __PYX_ERR(0, 694, __pyx_L1_error)
 
-  /* "Fortuna.pyx":678
+  /* "Fortuna.pyx":693
  * 
  *     def middle_gauss(self, *args, **kwargs):
  *         return flatten(             # <<<<<<<<<<<<<<
  *             self.data[_middle_gauss(self.size)], *args, flat=self.flat, **kwargs
  *         )
  */
-  __pyx_t_6 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_3, __pyx_t_2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 678, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_3, __pyx_t_2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 693, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_r = __pyx_t_6;
   __pyx_t_6 = 0;
   goto __pyx_L0;
 
-  /* "Fortuna.pyx":677
+  /* "Fortuna.pyx":692
  *             self.data[_front_gauss(self.size)], *args, flat=self.flat, **kwargs)
  * 
  *     def middle_gauss(self, *args, **kwargs):             # <<<<<<<<<<<<<<
  *         return flatten(
  *             self.data[_middle_gauss(self.size)], *args, flat=self.flat, **kwargs
  */
 
@@ -18105,15 +18670,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "Fortuna.pyx":682
+/* "Fortuna.pyx":697
  *         )
  * 
  *     def back_gauss(self, *args, **kwargs):             # <<<<<<<<<<<<<<
  *         return flatten(
  *             self.data[_back_gauss(self.size)], *args, flat=self.flat, **kwargs
  */
 
@@ -18178,32 +18743,32 @@
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_self)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 682, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 697, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
         const Py_ssize_t used_pos_args = (kwd_pos_args < 1) ? kwd_pos_args : 1;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, __pyx_v_kwargs, values + 0, used_pos_args, "back_gauss") < 0)) __PYX_ERR(0, 682, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, __pyx_v_kwargs, values + 0, used_pos_args, "back_gauss") < 0)) __PYX_ERR(0, 697, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs < 1)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
     }
     __pyx_v_self = values[0];
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("back_gauss", 0, 1, 1, __pyx_nargs); __PYX_ERR(0, 682, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("back_gauss", 0, 1, 1, __pyx_nargs); __PYX_ERR(0, 697, __pyx_L3_error)
   __pyx_L6_skip:;
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
@@ -18241,109 +18806,109 @@
   PyObject *__pyx_t_6 = NULL;
   PyObject *__pyx_t_7 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("back_gauss", 1);
 
-  /* "Fortuna.pyx":683
+  /* "Fortuna.pyx":698
  * 
  *     def back_gauss(self, *args, **kwargs):
  *         return flatten(             # <<<<<<<<<<<<<<
  *             self.data[_back_gauss(self.size)], *args, flat=self.flat, **kwargs
  *         )
  */
   __Pyx_XDECREF(__pyx_r);
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_flatten); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 683, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_flatten); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 698, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
 
-  /* "Fortuna.pyx":684
+  /* "Fortuna.pyx":699
  *     def back_gauss(self, *args, **kwargs):
  *         return flatten(
  *             self.data[_back_gauss(self.size)], *args, flat=self.flat, **kwargs             # <<<<<<<<<<<<<<
  *         )
  * 
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_data); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 684, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_data); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 699, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_size); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 684, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_size); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 699, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = __Pyx_PyInt_As_PY_LONG_LONG(__pyx_t_3); if (unlikely((__pyx_t_4 == (PY_LONG_LONG)-1) && PyErr_Occurred())) __PYX_ERR(0, 684, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyInt_As_PY_LONG_LONG(__pyx_t_3); if (unlikely((__pyx_t_4 == (PY_LONG_LONG)-1) && PyErr_Occurred())) __PYX_ERR(0, 699, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_t_5 = Storm::GetIndex::back_gauss(__pyx_t_4);
-  __pyx_t_3 = __Pyx_GetItemInt(__pyx_t_2, __pyx_t_5, PY_LONG_LONG, 1, __Pyx_PyInt_From_PY_LONG_LONG, 0, 1, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 684, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_GetItemInt(__pyx_t_2, __pyx_t_5, PY_LONG_LONG, 1, __Pyx_PyInt_From_PY_LONG_LONG, 0, 1, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 699, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "Fortuna.pyx":683
+  /* "Fortuna.pyx":698
  * 
  *     def back_gauss(self, *args, **kwargs):
  *         return flatten(             # <<<<<<<<<<<<<<
  *             self.data[_back_gauss(self.size)], *args, flat=self.flat, **kwargs
  *         )
  */
-  __pyx_t_2 = PyTuple_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 683, __pyx_L1_error)
+  __pyx_t_2 = PyTuple_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 698, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_GIVEREF(__pyx_t_3);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_t_3)) __PYX_ERR(0, 683, __pyx_L1_error);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_t_3)) __PYX_ERR(0, 698, __pyx_L1_error);
   __pyx_t_3 = 0;
 
-  /* "Fortuna.pyx":684
+  /* "Fortuna.pyx":699
  *     def back_gauss(self, *args, **kwargs):
  *         return flatten(
  *             self.data[_back_gauss(self.size)], *args, flat=self.flat, **kwargs             # <<<<<<<<<<<<<<
  *         )
  * 
  */
-  __pyx_t_3 = PyNumber_Add(__pyx_t_2, __pyx_v_args); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 683, __pyx_L1_error)
+  __pyx_t_3 = PyNumber_Add(__pyx_t_2, __pyx_v_args); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 698, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "Fortuna.pyx":683
+  /* "Fortuna.pyx":698
  * 
  *     def back_gauss(self, *args, **kwargs):
  *         return flatten(             # <<<<<<<<<<<<<<
  *             self.data[_back_gauss(self.size)], *args, flat=self.flat, **kwargs
  *         )
  */
-  __pyx_t_6 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 684, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 699, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
 
-  /* "Fortuna.pyx":684
+  /* "Fortuna.pyx":699
  *     def back_gauss(self, *args, **kwargs):
  *         return flatten(
  *             self.data[_back_gauss(self.size)], *args, flat=self.flat, **kwargs             # <<<<<<<<<<<<<<
  *         )
  * 
  */
-  __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_flat); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 684, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_flat); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 699, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  if (PyDict_SetItem(__pyx_t_6, __pyx_n_s_flat, __pyx_t_7) < 0) __PYX_ERR(0, 684, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_6, __pyx_n_s_flat, __pyx_t_7) < 0) __PYX_ERR(0, 699, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
   __pyx_t_2 = __pyx_t_6;
   __pyx_t_6 = 0;
-  if (__Pyx_MergeKeywords(__pyx_t_2, __pyx_v_kwargs) < 0) __PYX_ERR(0, 684, __pyx_L1_error)
+  if (__Pyx_MergeKeywords(__pyx_t_2, __pyx_v_kwargs) < 0) __PYX_ERR(0, 699, __pyx_L1_error)
 
-  /* "Fortuna.pyx":683
+  /* "Fortuna.pyx":698
  * 
  *     def back_gauss(self, *args, **kwargs):
  *         return flatten(             # <<<<<<<<<<<<<<
  *             self.data[_back_gauss(self.size)], *args, flat=self.flat, **kwargs
  *         )
  */
-  __pyx_t_6 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_3, __pyx_t_2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 683, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_3, __pyx_t_2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 698, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_r = __pyx_t_6;
   __pyx_t_6 = 0;
   goto __pyx_L0;
 
-  /* "Fortuna.pyx":682
+  /* "Fortuna.pyx":697
  *         )
  * 
  *     def back_gauss(self, *args, **kwargs):             # <<<<<<<<<<<<<<
  *         return flatten(
  *             self.data[_back_gauss(self.size)], *args, flat=self.flat, **kwargs
  */
 
@@ -18358,15 +18923,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "Fortuna.pyx":687
+/* "Fortuna.pyx":702
  *         )
  * 
  *     def quantum_gauss(self, *args, **kwargs):             # <<<<<<<<<<<<<<
  *         return flatten(
  *             self.data[_quantum_gauss(self.size)], *args, flat=self.flat, **kwargs
  */
 
@@ -18431,32 +18996,32 @@
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_self)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 687, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 702, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
         const Py_ssize_t used_pos_args = (kwd_pos_args < 1) ? kwd_pos_args : 1;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, __pyx_v_kwargs, values + 0, used_pos_args, "quantum_gauss") < 0)) __PYX_ERR(0, 687, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, __pyx_v_kwargs, values + 0, used_pos_args, "quantum_gauss") < 0)) __PYX_ERR(0, 702, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs < 1)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
     }
     __pyx_v_self = values[0];
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("quantum_gauss", 0, 1, 1, __pyx_nargs); __PYX_ERR(0, 687, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("quantum_gauss", 0, 1, 1, __pyx_nargs); __PYX_ERR(0, 702, __pyx_L3_error)
   __pyx_L6_skip:;
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
@@ -18494,109 +19059,109 @@
   PyObject *__pyx_t_6 = NULL;
   PyObject *__pyx_t_7 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("quantum_gauss", 1);
 
-  /* "Fortuna.pyx":688
+  /* "Fortuna.pyx":703
  * 
  *     def quantum_gauss(self, *args, **kwargs):
  *         return flatten(             # <<<<<<<<<<<<<<
  *             self.data[_quantum_gauss(self.size)], *args, flat=self.flat, **kwargs
  *         )
  */
   __Pyx_XDECREF(__pyx_r);
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_flatten); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 688, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_flatten); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 703, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
 
-  /* "Fortuna.pyx":689
+  /* "Fortuna.pyx":704
  *     def quantum_gauss(self, *args, **kwargs):
  *         return flatten(
  *             self.data[_quantum_gauss(self.size)], *args, flat=self.flat, **kwargs             # <<<<<<<<<<<<<<
  *         )
  * 
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_data); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 689, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_data); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 704, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_size); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 689, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_size); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 704, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = __Pyx_PyInt_As_PY_LONG_LONG(__pyx_t_3); if (unlikely((__pyx_t_4 == (PY_LONG_LONG)-1) && PyErr_Occurred())) __PYX_ERR(0, 689, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyInt_As_PY_LONG_LONG(__pyx_t_3); if (unlikely((__pyx_t_4 == (PY_LONG_LONG)-1) && PyErr_Occurred())) __PYX_ERR(0, 704, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_t_5 = Storm::GetIndex::quantum_gauss(__pyx_t_4);
-  __pyx_t_3 = __Pyx_GetItemInt(__pyx_t_2, __pyx_t_5, PY_LONG_LONG, 1, __Pyx_PyInt_From_PY_LONG_LONG, 0, 1, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 689, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_GetItemInt(__pyx_t_2, __pyx_t_5, PY_LONG_LONG, 1, __Pyx_PyInt_From_PY_LONG_LONG, 0, 1, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 704, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "Fortuna.pyx":688
+  /* "Fortuna.pyx":703
  * 
  *     def quantum_gauss(self, *args, **kwargs):
  *         return flatten(             # <<<<<<<<<<<<<<
  *             self.data[_quantum_gauss(self.size)], *args, flat=self.flat, **kwargs
  *         )
  */
-  __pyx_t_2 = PyTuple_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 688, __pyx_L1_error)
+  __pyx_t_2 = PyTuple_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 703, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_GIVEREF(__pyx_t_3);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_t_3)) __PYX_ERR(0, 688, __pyx_L1_error);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_t_3)) __PYX_ERR(0, 703, __pyx_L1_error);
   __pyx_t_3 = 0;
 
-  /* "Fortuna.pyx":689
+  /* "Fortuna.pyx":704
  *     def quantum_gauss(self, *args, **kwargs):
  *         return flatten(
  *             self.data[_quantum_gauss(self.size)], *args, flat=self.flat, **kwargs             # <<<<<<<<<<<<<<
  *         )
  * 
  */
-  __pyx_t_3 = PyNumber_Add(__pyx_t_2, __pyx_v_args); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 688, __pyx_L1_error)
+  __pyx_t_3 = PyNumber_Add(__pyx_t_2, __pyx_v_args); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 703, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "Fortuna.pyx":688
+  /* "Fortuna.pyx":703
  * 
  *     def quantum_gauss(self, *args, **kwargs):
  *         return flatten(             # <<<<<<<<<<<<<<
  *             self.data[_quantum_gauss(self.size)], *args, flat=self.flat, **kwargs
  *         )
  */
-  __pyx_t_6 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 689, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 704, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
 
-  /* "Fortuna.pyx":689
+  /* "Fortuna.pyx":704
  *     def quantum_gauss(self, *args, **kwargs):
  *         return flatten(
  *             self.data[_quantum_gauss(self.size)], *args, flat=self.flat, **kwargs             # <<<<<<<<<<<<<<
  *         )
  * 
  */
-  __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_flat); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 689, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_flat); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 704, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  if (PyDict_SetItem(__pyx_t_6, __pyx_n_s_flat, __pyx_t_7) < 0) __PYX_ERR(0, 689, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_6, __pyx_n_s_flat, __pyx_t_7) < 0) __PYX_ERR(0, 704, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
   __pyx_t_2 = __pyx_t_6;
   __pyx_t_6 = 0;
-  if (__Pyx_MergeKeywords(__pyx_t_2, __pyx_v_kwargs) < 0) __PYX_ERR(0, 689, __pyx_L1_error)
+  if (__Pyx_MergeKeywords(__pyx_t_2, __pyx_v_kwargs) < 0) __PYX_ERR(0, 704, __pyx_L1_error)
 
-  /* "Fortuna.pyx":688
+  /* "Fortuna.pyx":703
  * 
  *     def quantum_gauss(self, *args, **kwargs):
  *         return flatten(             # <<<<<<<<<<<<<<
  *             self.data[_quantum_gauss(self.size)], *args, flat=self.flat, **kwargs
  *         )
  */
-  __pyx_t_6 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_3, __pyx_t_2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 688, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_3, __pyx_t_2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 703, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_r = __pyx_t_6;
   __pyx_t_6 = 0;
   goto __pyx_L0;
 
-  /* "Fortuna.pyx":687
+  /* "Fortuna.pyx":702
  *         )
  * 
  *     def quantum_gauss(self, *args, **kwargs):             # <<<<<<<<<<<<<<
  *         return flatten(
  *             self.data[_quantum_gauss(self.size)], *args, flat=self.flat, **kwargs
  */
 
@@ -18611,15 +19176,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "Fortuna.pyx":692
+/* "Fortuna.pyx":707
  *         )
  * 
  *     def front_poisson(self, *args, **kwargs):             # <<<<<<<<<<<<<<
  *         return flatten(
  *             self.data[_front_poisson(self.size)], *args, flat=self.flat, **kwargs
  */
 
@@ -18684,32 +19249,32 @@
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_self)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 692, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 707, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
         const Py_ssize_t used_pos_args = (kwd_pos_args < 1) ? kwd_pos_args : 1;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, __pyx_v_kwargs, values + 0, used_pos_args, "front_poisson") < 0)) __PYX_ERR(0, 692, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, __pyx_v_kwargs, values + 0, used_pos_args, "front_poisson") < 0)) __PYX_ERR(0, 707, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs < 1)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
     }
     __pyx_v_self = values[0];
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("front_poisson", 0, 1, 1, __pyx_nargs); __PYX_ERR(0, 692, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("front_poisson", 0, 1, 1, __pyx_nargs); __PYX_ERR(0, 707, __pyx_L3_error)
   __pyx_L6_skip:;
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
@@ -18747,109 +19312,109 @@
   PyObject *__pyx_t_6 = NULL;
   PyObject *__pyx_t_7 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("front_poisson", 1);
 
-  /* "Fortuna.pyx":693
+  /* "Fortuna.pyx":708
  * 
  *     def front_poisson(self, *args, **kwargs):
  *         return flatten(             # <<<<<<<<<<<<<<
  *             self.data[_front_poisson(self.size)], *args, flat=self.flat, **kwargs
  *         )
  */
   __Pyx_XDECREF(__pyx_r);
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_flatten); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 693, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_flatten); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 708, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
 
-  /* "Fortuna.pyx":694
+  /* "Fortuna.pyx":709
  *     def front_poisson(self, *args, **kwargs):
  *         return flatten(
  *             self.data[_front_poisson(self.size)], *args, flat=self.flat, **kwargs             # <<<<<<<<<<<<<<
  *         )
  * 
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_data); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 694, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_data); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 709, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_size); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 694, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_size); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 709, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = __Pyx_PyInt_As_PY_LONG_LONG(__pyx_t_3); if (unlikely((__pyx_t_4 == (PY_LONG_LONG)-1) && PyErr_Occurred())) __PYX_ERR(0, 694, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyInt_As_PY_LONG_LONG(__pyx_t_3); if (unlikely((__pyx_t_4 == (PY_LONG_LONG)-1) && PyErr_Occurred())) __PYX_ERR(0, 709, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_t_5 = Storm::GetIndex::front_poisson(__pyx_t_4);
-  __pyx_t_3 = __Pyx_GetItemInt(__pyx_t_2, __pyx_t_5, PY_LONG_LONG, 1, __Pyx_PyInt_From_PY_LONG_LONG, 0, 1, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 694, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_GetItemInt(__pyx_t_2, __pyx_t_5, PY_LONG_LONG, 1, __Pyx_PyInt_From_PY_LONG_LONG, 0, 1, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 709, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "Fortuna.pyx":693
+  /* "Fortuna.pyx":708
  * 
  *     def front_poisson(self, *args, **kwargs):
  *         return flatten(             # <<<<<<<<<<<<<<
  *             self.data[_front_poisson(self.size)], *args, flat=self.flat, **kwargs
  *         )
  */
-  __pyx_t_2 = PyTuple_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 693, __pyx_L1_error)
+  __pyx_t_2 = PyTuple_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 708, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_GIVEREF(__pyx_t_3);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_t_3)) __PYX_ERR(0, 693, __pyx_L1_error);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_t_3)) __PYX_ERR(0, 708, __pyx_L1_error);
   __pyx_t_3 = 0;
 
-  /* "Fortuna.pyx":694
+  /* "Fortuna.pyx":709
  *     def front_poisson(self, *args, **kwargs):
  *         return flatten(
  *             self.data[_front_poisson(self.size)], *args, flat=self.flat, **kwargs             # <<<<<<<<<<<<<<
  *         )
  * 
  */
-  __pyx_t_3 = PyNumber_Add(__pyx_t_2, __pyx_v_args); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 693, __pyx_L1_error)
+  __pyx_t_3 = PyNumber_Add(__pyx_t_2, __pyx_v_args); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 708, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "Fortuna.pyx":693
+  /* "Fortuna.pyx":708
  * 
  *     def front_poisson(self, *args, **kwargs):
  *         return flatten(             # <<<<<<<<<<<<<<
  *             self.data[_front_poisson(self.size)], *args, flat=self.flat, **kwargs
  *         )
  */
-  __pyx_t_6 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 694, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 709, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
 
-  /* "Fortuna.pyx":694
+  /* "Fortuna.pyx":709
  *     def front_poisson(self, *args, **kwargs):
  *         return flatten(
  *             self.data[_front_poisson(self.size)], *args, flat=self.flat, **kwargs             # <<<<<<<<<<<<<<
  *         )
  * 
  */
-  __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_flat); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 694, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_flat); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 709, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  if (PyDict_SetItem(__pyx_t_6, __pyx_n_s_flat, __pyx_t_7) < 0) __PYX_ERR(0, 694, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_6, __pyx_n_s_flat, __pyx_t_7) < 0) __PYX_ERR(0, 709, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
   __pyx_t_2 = __pyx_t_6;
   __pyx_t_6 = 0;
-  if (__Pyx_MergeKeywords(__pyx_t_2, __pyx_v_kwargs) < 0) __PYX_ERR(0, 694, __pyx_L1_error)
+  if (__Pyx_MergeKeywords(__pyx_t_2, __pyx_v_kwargs) < 0) __PYX_ERR(0, 709, __pyx_L1_error)
 
-  /* "Fortuna.pyx":693
+  /* "Fortuna.pyx":708
  * 
  *     def front_poisson(self, *args, **kwargs):
  *         return flatten(             # <<<<<<<<<<<<<<
  *             self.data[_front_poisson(self.size)], *args, flat=self.flat, **kwargs
  *         )
  */
-  __pyx_t_6 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_3, __pyx_t_2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 693, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_3, __pyx_t_2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 708, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_r = __pyx_t_6;
   __pyx_t_6 = 0;
   goto __pyx_L0;
 
-  /* "Fortuna.pyx":692
+  /* "Fortuna.pyx":707
  *         )
  * 
  *     def front_poisson(self, *args, **kwargs):             # <<<<<<<<<<<<<<
  *         return flatten(
  *             self.data[_front_poisson(self.size)], *args, flat=self.flat, **kwargs
  */
 
@@ -18864,15 +19429,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "Fortuna.pyx":697
+/* "Fortuna.pyx":712
  *         )
  * 
  *     def middle_poisson(self, *args, **kwargs):             # <<<<<<<<<<<<<<
  *         return flatten(
  *             self.data[_middle_poisson(self.size)], *args, flat=self.flat, **kwargs
  */
 
@@ -18937,32 +19502,32 @@
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_self)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 697, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 712, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
         const Py_ssize_t used_pos_args = (kwd_pos_args < 1) ? kwd_pos_args : 1;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, __pyx_v_kwargs, values + 0, used_pos_args, "middle_poisson") < 0)) __PYX_ERR(0, 697, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, __pyx_v_kwargs, values + 0, used_pos_args, "middle_poisson") < 0)) __PYX_ERR(0, 712, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs < 1)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
     }
     __pyx_v_self = values[0];
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("middle_poisson", 0, 1, 1, __pyx_nargs); __PYX_ERR(0, 697, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("middle_poisson", 0, 1, 1, __pyx_nargs); __PYX_ERR(0, 712, __pyx_L3_error)
   __pyx_L6_skip:;
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
@@ -19000,109 +19565,109 @@
   PyObject *__pyx_t_6 = NULL;
   PyObject *__pyx_t_7 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("middle_poisson", 1);
 
-  /* "Fortuna.pyx":698
+  /* "Fortuna.pyx":713
  * 
  *     def middle_poisson(self, *args, **kwargs):
  *         return flatten(             # <<<<<<<<<<<<<<
  *             self.data[_middle_poisson(self.size)], *args, flat=self.flat, **kwargs
  *         )
  */
   __Pyx_XDECREF(__pyx_r);
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_flatten); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 698, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_flatten); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 713, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
 
-  /* "Fortuna.pyx":699
+  /* "Fortuna.pyx":714
  *     def middle_poisson(self, *args, **kwargs):
  *         return flatten(
  *             self.data[_middle_poisson(self.size)], *args, flat=self.flat, **kwargs             # <<<<<<<<<<<<<<
  *         )
  * 
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_data); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 699, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_data); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 714, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_size); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 699, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_size); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 714, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = __Pyx_PyInt_As_PY_LONG_LONG(__pyx_t_3); if (unlikely((__pyx_t_4 == (PY_LONG_LONG)-1) && PyErr_Occurred())) __PYX_ERR(0, 699, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyInt_As_PY_LONG_LONG(__pyx_t_3); if (unlikely((__pyx_t_4 == (PY_LONG_LONG)-1) && PyErr_Occurred())) __PYX_ERR(0, 714, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_t_5 = Storm::GetIndex::middle_poisson(__pyx_t_4);
-  __pyx_t_3 = __Pyx_GetItemInt(__pyx_t_2, __pyx_t_5, PY_LONG_LONG, 1, __Pyx_PyInt_From_PY_LONG_LONG, 0, 1, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 699, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_GetItemInt(__pyx_t_2, __pyx_t_5, PY_LONG_LONG, 1, __Pyx_PyInt_From_PY_LONG_LONG, 0, 1, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 714, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "Fortuna.pyx":698
+  /* "Fortuna.pyx":713
  * 
  *     def middle_poisson(self, *args, **kwargs):
  *         return flatten(             # <<<<<<<<<<<<<<
  *             self.data[_middle_poisson(self.size)], *args, flat=self.flat, **kwargs
  *         )
  */
-  __pyx_t_2 = PyTuple_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 698, __pyx_L1_error)
+  __pyx_t_2 = PyTuple_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 713, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_GIVEREF(__pyx_t_3);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_t_3)) __PYX_ERR(0, 698, __pyx_L1_error);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_t_3)) __PYX_ERR(0, 713, __pyx_L1_error);
   __pyx_t_3 = 0;
 
-  /* "Fortuna.pyx":699
+  /* "Fortuna.pyx":714
  *     def middle_poisson(self, *args, **kwargs):
  *         return flatten(
  *             self.data[_middle_poisson(self.size)], *args, flat=self.flat, **kwargs             # <<<<<<<<<<<<<<
  *         )
  * 
  */
-  __pyx_t_3 = PyNumber_Add(__pyx_t_2, __pyx_v_args); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 698, __pyx_L1_error)
+  __pyx_t_3 = PyNumber_Add(__pyx_t_2, __pyx_v_args); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 713, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "Fortuna.pyx":698
+  /* "Fortuna.pyx":713
  * 
  *     def middle_poisson(self, *args, **kwargs):
  *         return flatten(             # <<<<<<<<<<<<<<
  *             self.data[_middle_poisson(self.size)], *args, flat=self.flat, **kwargs
  *         )
  */
-  __pyx_t_6 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 699, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 714, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
 
-  /* "Fortuna.pyx":699
+  /* "Fortuna.pyx":714
  *     def middle_poisson(self, *args, **kwargs):
  *         return flatten(
  *             self.data[_middle_poisson(self.size)], *args, flat=self.flat, **kwargs             # <<<<<<<<<<<<<<
  *         )
  * 
  */
-  __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_flat); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 699, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_flat); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 714, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  if (PyDict_SetItem(__pyx_t_6, __pyx_n_s_flat, __pyx_t_7) < 0) __PYX_ERR(0, 699, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_6, __pyx_n_s_flat, __pyx_t_7) < 0) __PYX_ERR(0, 714, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
   __pyx_t_2 = __pyx_t_6;
   __pyx_t_6 = 0;
-  if (__Pyx_MergeKeywords(__pyx_t_2, __pyx_v_kwargs) < 0) __PYX_ERR(0, 699, __pyx_L1_error)
+  if (__Pyx_MergeKeywords(__pyx_t_2, __pyx_v_kwargs) < 0) __PYX_ERR(0, 714, __pyx_L1_error)
 
-  /* "Fortuna.pyx":698
+  /* "Fortuna.pyx":713
  * 
  *     def middle_poisson(self, *args, **kwargs):
  *         return flatten(             # <<<<<<<<<<<<<<
  *             self.data[_middle_poisson(self.size)], *args, flat=self.flat, **kwargs
  *         )
  */
-  __pyx_t_6 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_3, __pyx_t_2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 698, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_3, __pyx_t_2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 713, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_r = __pyx_t_6;
   __pyx_t_6 = 0;
   goto __pyx_L0;
 
-  /* "Fortuna.pyx":697
+  /* "Fortuna.pyx":712
  *         )
  * 
  *     def middle_poisson(self, *args, **kwargs):             # <<<<<<<<<<<<<<
  *         return flatten(
  *             self.data[_middle_poisson(self.size)], *args, flat=self.flat, **kwargs
  */
 
@@ -19117,15 +19682,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "Fortuna.pyx":702
+/* "Fortuna.pyx":717
  *         )
  * 
  *     def back_poisson(self, *args, **kwargs):             # <<<<<<<<<<<<<<
  *         return flatten(
  *             self.data[_back_poisson(self.size)], *args, flat=self.flat, **kwargs
  */
 
@@ -19190,32 +19755,32 @@
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_self)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 702, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 717, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
         const Py_ssize_t used_pos_args = (kwd_pos_args < 1) ? kwd_pos_args : 1;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, __pyx_v_kwargs, values + 0, used_pos_args, "back_poisson") < 0)) __PYX_ERR(0, 702, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, __pyx_v_kwargs, values + 0, used_pos_args, "back_poisson") < 0)) __PYX_ERR(0, 717, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs < 1)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
     }
     __pyx_v_self = values[0];
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("back_poisson", 0, 1, 1, __pyx_nargs); __PYX_ERR(0, 702, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("back_poisson", 0, 1, 1, __pyx_nargs); __PYX_ERR(0, 717, __pyx_L3_error)
   __pyx_L6_skip:;
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
@@ -19253,109 +19818,109 @@
   PyObject *__pyx_t_6 = NULL;
   PyObject *__pyx_t_7 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("back_poisson", 1);
 
-  /* "Fortuna.pyx":703
+  /* "Fortuna.pyx":718
  * 
  *     def back_poisson(self, *args, **kwargs):
  *         return flatten(             # <<<<<<<<<<<<<<
  *             self.data[_back_poisson(self.size)], *args, flat=self.flat, **kwargs
  *         )
  */
   __Pyx_XDECREF(__pyx_r);
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_flatten); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 703, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_flatten); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 718, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
 
-  /* "Fortuna.pyx":704
+  /* "Fortuna.pyx":719
  *     def back_poisson(self, *args, **kwargs):
  *         return flatten(
  *             self.data[_back_poisson(self.size)], *args, flat=self.flat, **kwargs             # <<<<<<<<<<<<<<
  *         )
  * 
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_data); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 704, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_data); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 719, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_size); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 704, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_size); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 719, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = __Pyx_PyInt_As_PY_LONG_LONG(__pyx_t_3); if (unlikely((__pyx_t_4 == (PY_LONG_LONG)-1) && PyErr_Occurred())) __PYX_ERR(0, 704, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyInt_As_PY_LONG_LONG(__pyx_t_3); if (unlikely((__pyx_t_4 == (PY_LONG_LONG)-1) && PyErr_Occurred())) __PYX_ERR(0, 719, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_t_5 = Storm::GetIndex::back_poisson(__pyx_t_4);
-  __pyx_t_3 = __Pyx_GetItemInt(__pyx_t_2, __pyx_t_5, PY_LONG_LONG, 1, __Pyx_PyInt_From_PY_LONG_LONG, 0, 1, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 704, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_GetItemInt(__pyx_t_2, __pyx_t_5, PY_LONG_LONG, 1, __Pyx_PyInt_From_PY_LONG_LONG, 0, 1, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 719, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "Fortuna.pyx":703
+  /* "Fortuna.pyx":718
  * 
  *     def back_poisson(self, *args, **kwargs):
  *         return flatten(             # <<<<<<<<<<<<<<
  *             self.data[_back_poisson(self.size)], *args, flat=self.flat, **kwargs
  *         )
  */
-  __pyx_t_2 = PyTuple_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 703, __pyx_L1_error)
+  __pyx_t_2 = PyTuple_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 718, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_GIVEREF(__pyx_t_3);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_t_3)) __PYX_ERR(0, 703, __pyx_L1_error);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_t_3)) __PYX_ERR(0, 718, __pyx_L1_error);
   __pyx_t_3 = 0;
 
-  /* "Fortuna.pyx":704
+  /* "Fortuna.pyx":719
  *     def back_poisson(self, *args, **kwargs):
  *         return flatten(
  *             self.data[_back_poisson(self.size)], *args, flat=self.flat, **kwargs             # <<<<<<<<<<<<<<
  *         )
  * 
  */
-  __pyx_t_3 = PyNumber_Add(__pyx_t_2, __pyx_v_args); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 703, __pyx_L1_error)
+  __pyx_t_3 = PyNumber_Add(__pyx_t_2, __pyx_v_args); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 718, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "Fortuna.pyx":703
+  /* "Fortuna.pyx":718
  * 
  *     def back_poisson(self, *args, **kwargs):
  *         return flatten(             # <<<<<<<<<<<<<<
  *             self.data[_back_poisson(self.size)], *args, flat=self.flat, **kwargs
  *         )
  */
-  __pyx_t_6 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 704, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 719, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
 
-  /* "Fortuna.pyx":704
+  /* "Fortuna.pyx":719
  *     def back_poisson(self, *args, **kwargs):
  *         return flatten(
  *             self.data[_back_poisson(self.size)], *args, flat=self.flat, **kwargs             # <<<<<<<<<<<<<<
  *         )
  * 
  */
-  __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_flat); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 704, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_flat); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 719, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  if (PyDict_SetItem(__pyx_t_6, __pyx_n_s_flat, __pyx_t_7) < 0) __PYX_ERR(0, 704, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_6, __pyx_n_s_flat, __pyx_t_7) < 0) __PYX_ERR(0, 719, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
   __pyx_t_2 = __pyx_t_6;
   __pyx_t_6 = 0;
-  if (__Pyx_MergeKeywords(__pyx_t_2, __pyx_v_kwargs) < 0) __PYX_ERR(0, 704, __pyx_L1_error)
+  if (__Pyx_MergeKeywords(__pyx_t_2, __pyx_v_kwargs) < 0) __PYX_ERR(0, 719, __pyx_L1_error)
 
-  /* "Fortuna.pyx":703
+  /* "Fortuna.pyx":718
  * 
  *     def back_poisson(self, *args, **kwargs):
  *         return flatten(             # <<<<<<<<<<<<<<
  *             self.data[_back_poisson(self.size)], *args, flat=self.flat, **kwargs
  *         )
  */
-  __pyx_t_6 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_3, __pyx_t_2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 703, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_3, __pyx_t_2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 718, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_r = __pyx_t_6;
   __pyx_t_6 = 0;
   goto __pyx_L0;
 
-  /* "Fortuna.pyx":702
+  /* "Fortuna.pyx":717
  *         )
  * 
  *     def back_poisson(self, *args, **kwargs):             # <<<<<<<<<<<<<<
  *         return flatten(
  *             self.data[_back_poisson(self.size)], *args, flat=self.flat, **kwargs
  */
 
@@ -19370,15 +19935,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "Fortuna.pyx":707
+/* "Fortuna.pyx":722
  *         )
  * 
  *     def quantum_poisson(self, *args, **kwargs):             # <<<<<<<<<<<<<<
  *         return flatten(
  *             self.data[_quantum_poisson(self.size)], *args, flat=self.flat, **kwargs
  */
 
@@ -19443,32 +20008,32 @@
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_self)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 707, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 722, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
         const Py_ssize_t used_pos_args = (kwd_pos_args < 1) ? kwd_pos_args : 1;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, __pyx_v_kwargs, values + 0, used_pos_args, "quantum_poisson") < 0)) __PYX_ERR(0, 707, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, __pyx_v_kwargs, values + 0, used_pos_args, "quantum_poisson") < 0)) __PYX_ERR(0, 722, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs < 1)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
     }
     __pyx_v_self = values[0];
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("quantum_poisson", 0, 1, 1, __pyx_nargs); __PYX_ERR(0, 707, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("quantum_poisson", 0, 1, 1, __pyx_nargs); __PYX_ERR(0, 722, __pyx_L3_error)
   __pyx_L6_skip:;
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
@@ -19506,109 +20071,109 @@
   PyObject *__pyx_t_6 = NULL;
   PyObject *__pyx_t_7 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("quantum_poisson", 1);
 
-  /* "Fortuna.pyx":708
+  /* "Fortuna.pyx":723
  * 
  *     def quantum_poisson(self, *args, **kwargs):
  *         return flatten(             # <<<<<<<<<<<<<<
  *             self.data[_quantum_poisson(self.size)], *args, flat=self.flat, **kwargs
  *         )
  */
   __Pyx_XDECREF(__pyx_r);
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_flatten); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 708, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_flatten); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 723, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
 
-  /* "Fortuna.pyx":709
+  /* "Fortuna.pyx":724
  *     def quantum_poisson(self, *args, **kwargs):
  *         return flatten(
  *             self.data[_quantum_poisson(self.size)], *args, flat=self.flat, **kwargs             # <<<<<<<<<<<<<<
  *         )
  * 
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_data); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 709, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_data); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 724, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_size); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 709, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_size); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 724, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = __Pyx_PyInt_As_PY_LONG_LONG(__pyx_t_3); if (unlikely((__pyx_t_4 == (PY_LONG_LONG)-1) && PyErr_Occurred())) __PYX_ERR(0, 709, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyInt_As_PY_LONG_LONG(__pyx_t_3); if (unlikely((__pyx_t_4 == (PY_LONG_LONG)-1) && PyErr_Occurred())) __PYX_ERR(0, 724, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_t_5 = Storm::GetIndex::quantum_poisson(__pyx_t_4);
-  __pyx_t_3 = __Pyx_GetItemInt(__pyx_t_2, __pyx_t_5, PY_LONG_LONG, 1, __Pyx_PyInt_From_PY_LONG_LONG, 0, 1, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 709, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_GetItemInt(__pyx_t_2, __pyx_t_5, PY_LONG_LONG, 1, __Pyx_PyInt_From_PY_LONG_LONG, 0, 1, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 724, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "Fortuna.pyx":708
+  /* "Fortuna.pyx":723
  * 
  *     def quantum_poisson(self, *args, **kwargs):
  *         return flatten(             # <<<<<<<<<<<<<<
  *             self.data[_quantum_poisson(self.size)], *args, flat=self.flat, **kwargs
  *         )
  */
-  __pyx_t_2 = PyTuple_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 708, __pyx_L1_error)
+  __pyx_t_2 = PyTuple_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 723, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_GIVEREF(__pyx_t_3);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_t_3)) __PYX_ERR(0, 708, __pyx_L1_error);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_t_3)) __PYX_ERR(0, 723, __pyx_L1_error);
   __pyx_t_3 = 0;
 
-  /* "Fortuna.pyx":709
+  /* "Fortuna.pyx":724
  *     def quantum_poisson(self, *args, **kwargs):
  *         return flatten(
  *             self.data[_quantum_poisson(self.size)], *args, flat=self.flat, **kwargs             # <<<<<<<<<<<<<<
  *         )
  * 
  */
-  __pyx_t_3 = PyNumber_Add(__pyx_t_2, __pyx_v_args); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 708, __pyx_L1_error)
+  __pyx_t_3 = PyNumber_Add(__pyx_t_2, __pyx_v_args); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 723, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "Fortuna.pyx":708
+  /* "Fortuna.pyx":723
  * 
  *     def quantum_poisson(self, *args, **kwargs):
  *         return flatten(             # <<<<<<<<<<<<<<
  *             self.data[_quantum_poisson(self.size)], *args, flat=self.flat, **kwargs
  *         )
  */
-  __pyx_t_6 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 709, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 724, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
 
-  /* "Fortuna.pyx":709
+  /* "Fortuna.pyx":724
  *     def quantum_poisson(self, *args, **kwargs):
  *         return flatten(
  *             self.data[_quantum_poisson(self.size)], *args, flat=self.flat, **kwargs             # <<<<<<<<<<<<<<
  *         )
  * 
  */
-  __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_flat); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 709, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_flat); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 724, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  if (PyDict_SetItem(__pyx_t_6, __pyx_n_s_flat, __pyx_t_7) < 0) __PYX_ERR(0, 709, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_6, __pyx_n_s_flat, __pyx_t_7) < 0) __PYX_ERR(0, 724, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
   __pyx_t_2 = __pyx_t_6;
   __pyx_t_6 = 0;
-  if (__Pyx_MergeKeywords(__pyx_t_2, __pyx_v_kwargs) < 0) __PYX_ERR(0, 709, __pyx_L1_error)
+  if (__Pyx_MergeKeywords(__pyx_t_2, __pyx_v_kwargs) < 0) __PYX_ERR(0, 724, __pyx_L1_error)
 
-  /* "Fortuna.pyx":708
+  /* "Fortuna.pyx":723
  * 
  *     def quantum_poisson(self, *args, **kwargs):
  *         return flatten(             # <<<<<<<<<<<<<<
  *             self.data[_quantum_poisson(self.size)], *args, flat=self.flat, **kwargs
  *         )
  */
-  __pyx_t_6 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_3, __pyx_t_2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 708, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_3, __pyx_t_2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 723, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_r = __pyx_t_6;
   __pyx_t_6 = 0;
   goto __pyx_L0;
 
-  /* "Fortuna.pyx":707
+  /* "Fortuna.pyx":722
  *         )
  * 
  *     def quantum_poisson(self, *args, **kwargs):             # <<<<<<<<<<<<<<
  *         return flatten(
  *             self.data[_quantum_poisson(self.size)], *args, flat=self.flat, **kwargs
  */
 
@@ -19623,15 +20188,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "Fortuna.pyx":712
+/* "Fortuna.pyx":727
  *         )
  * 
  *     def quantum_monty(self, *args, **kwargs):             # <<<<<<<<<<<<<<
  *         return flatten(
  *             self.data[_quantum_monty(self.size)], *args, flat=self.flat, **kwargs
  */
 
@@ -19696,32 +20261,32 @@
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_self)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 712, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 727, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
         const Py_ssize_t used_pos_args = (kwd_pos_args < 1) ? kwd_pos_args : 1;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, __pyx_v_kwargs, values + 0, used_pos_args, "quantum_monty") < 0)) __PYX_ERR(0, 712, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, __pyx_v_kwargs, values + 0, used_pos_args, "quantum_monty") < 0)) __PYX_ERR(0, 727, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs < 1)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
     }
     __pyx_v_self = values[0];
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("quantum_monty", 0, 1, 1, __pyx_nargs); __PYX_ERR(0, 712, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("quantum_monty", 0, 1, 1, __pyx_nargs); __PYX_ERR(0, 727, __pyx_L3_error)
   __pyx_L6_skip:;
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
@@ -19759,109 +20324,109 @@
   PyObject *__pyx_t_6 = NULL;
   PyObject *__pyx_t_7 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("quantum_monty", 1);
 
-  /* "Fortuna.pyx":713
+  /* "Fortuna.pyx":728
  * 
  *     def quantum_monty(self, *args, **kwargs):
  *         return flatten(             # <<<<<<<<<<<<<<
  *             self.data[_quantum_monty(self.size)], *args, flat=self.flat, **kwargs
  *         )
  */
   __Pyx_XDECREF(__pyx_r);
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_flatten); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 713, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_flatten); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 728, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
 
-  /* "Fortuna.pyx":714
+  /* "Fortuna.pyx":729
  *     def quantum_monty(self, *args, **kwargs):
  *         return flatten(
  *             self.data[_quantum_monty(self.size)], *args, flat=self.flat, **kwargs             # <<<<<<<<<<<<<<
  *         )
  * 
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_data); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 714, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_data); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 729, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_size); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 714, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_size); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 729, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = __Pyx_PyInt_As_PY_LONG_LONG(__pyx_t_3); if (unlikely((__pyx_t_4 == (PY_LONG_LONG)-1) && PyErr_Occurred())) __PYX_ERR(0, 714, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyInt_As_PY_LONG_LONG(__pyx_t_3); if (unlikely((__pyx_t_4 == (PY_LONG_LONG)-1) && PyErr_Occurred())) __PYX_ERR(0, 729, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_t_5 = Storm::GetIndex::quantum_monty(__pyx_t_4);
-  __pyx_t_3 = __Pyx_GetItemInt(__pyx_t_2, __pyx_t_5, PY_LONG_LONG, 1, __Pyx_PyInt_From_PY_LONG_LONG, 0, 1, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 714, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_GetItemInt(__pyx_t_2, __pyx_t_5, PY_LONG_LONG, 1, __Pyx_PyInt_From_PY_LONG_LONG, 0, 1, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 729, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "Fortuna.pyx":713
+  /* "Fortuna.pyx":728
  * 
  *     def quantum_monty(self, *args, **kwargs):
  *         return flatten(             # <<<<<<<<<<<<<<
  *             self.data[_quantum_monty(self.size)], *args, flat=self.flat, **kwargs
  *         )
  */
-  __pyx_t_2 = PyTuple_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 713, __pyx_L1_error)
+  __pyx_t_2 = PyTuple_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 728, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_GIVEREF(__pyx_t_3);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_t_3)) __PYX_ERR(0, 713, __pyx_L1_error);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_t_3)) __PYX_ERR(0, 728, __pyx_L1_error);
   __pyx_t_3 = 0;
 
-  /* "Fortuna.pyx":714
+  /* "Fortuna.pyx":729
  *     def quantum_monty(self, *args, **kwargs):
  *         return flatten(
  *             self.data[_quantum_monty(self.size)], *args, flat=self.flat, **kwargs             # <<<<<<<<<<<<<<
  *         )
  * 
  */
-  __pyx_t_3 = PyNumber_Add(__pyx_t_2, __pyx_v_args); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 713, __pyx_L1_error)
+  __pyx_t_3 = PyNumber_Add(__pyx_t_2, __pyx_v_args); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 728, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "Fortuna.pyx":713
+  /* "Fortuna.pyx":728
  * 
  *     def quantum_monty(self, *args, **kwargs):
  *         return flatten(             # <<<<<<<<<<<<<<
  *             self.data[_quantum_monty(self.size)], *args, flat=self.flat, **kwargs
  *         )
  */
-  __pyx_t_6 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 714, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 729, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
 
-  /* "Fortuna.pyx":714
+  /* "Fortuna.pyx":729
  *     def quantum_monty(self, *args, **kwargs):
  *         return flatten(
  *             self.data[_quantum_monty(self.size)], *args, flat=self.flat, **kwargs             # <<<<<<<<<<<<<<
  *         )
  * 
  */
-  __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_flat); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 714, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_flat); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 729, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  if (PyDict_SetItem(__pyx_t_6, __pyx_n_s_flat, __pyx_t_7) < 0) __PYX_ERR(0, 714, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_6, __pyx_n_s_flat, __pyx_t_7) < 0) __PYX_ERR(0, 729, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
   __pyx_t_2 = __pyx_t_6;
   __pyx_t_6 = 0;
-  if (__Pyx_MergeKeywords(__pyx_t_2, __pyx_v_kwargs) < 0) __PYX_ERR(0, 714, __pyx_L1_error)
+  if (__Pyx_MergeKeywords(__pyx_t_2, __pyx_v_kwargs) < 0) __PYX_ERR(0, 729, __pyx_L1_error)
 
-  /* "Fortuna.pyx":713
+  /* "Fortuna.pyx":728
  * 
  *     def quantum_monty(self, *args, **kwargs):
  *         return flatten(             # <<<<<<<<<<<<<<
  *             self.data[_quantum_monty(self.size)], *args, flat=self.flat, **kwargs
  *         )
  */
-  __pyx_t_6 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_3, __pyx_t_2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 713, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_3, __pyx_t_2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 728, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_r = __pyx_t_6;
   __pyx_t_6 = 0;
   goto __pyx_L0;
 
-  /* "Fortuna.pyx":712
+  /* "Fortuna.pyx":727
  *         )
  * 
  *     def quantum_monty(self, *args, **kwargs):             # <<<<<<<<<<<<<<
  *         return flatten(
  *             self.data[_quantum_monty(self.size)], *args, flat=self.flat, **kwargs
  */
 
@@ -19876,15 +20441,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "Fortuna.pyx":741
+/* "Fortuna.pyx":756
  *                  "double_cycle", "cycle")
  * 
  *     def __init__(self,             # <<<<<<<<<<<<<<
  *                  matrix_data: Dict,
  *                  key_bias: str = "front_linear",
  */
 
@@ -19930,15 +20495,15 @@
   #endif
   __pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
   {
     PyObject **__pyx_pyargnames[] = {&__pyx_n_s_self,&__pyx_n_s_matrix_data,&__pyx_n_s_key_bias,&__pyx_n_s_val_bias,&__pyx_n_s_flat,0};
     values[2] = __Pyx_Arg_NewRef_FASTCALL(((PyObject*)((PyObject*)__pyx_n_u_front_linear)));
     values[3] = __Pyx_Arg_NewRef_FASTCALL(((PyObject*)((PyObject*)__pyx_n_u_truffle_shuffle)));
 
-    /* "Fortuna.pyx":745
+    /* "Fortuna.pyx":760
  *                  key_bias: str = "front_linear",
  *                  val_bias: str = "truffle_shuffle",
  *                  flat: bool = True):             # <<<<<<<<<<<<<<
  *         """
  *         @param matrix_data : Dictionary of Value Sequences.
  */
     values[4] = __Pyx_Arg_NewRef_FASTCALL(((PyObject *)((PyObject *)Py_True)));
@@ -19961,51 +20526,51 @@
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_self)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 741, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 756, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_matrix_data)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[1]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 741, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 756, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("__init__", 0, 2, 5, 1); __PYX_ERR(0, 741, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__init__", 0, 2, 5, 1); __PYX_ERR(0, 756, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (kw_args > 0) {
           PyObject* value = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_key_bias);
           if (value) { values[2] = __Pyx_Arg_NewRef_FASTCALL(value); kw_args--; }
-          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 741, __pyx_L3_error)
+          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 756, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  3:
         if (kw_args > 0) {
           PyObject* value = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_val_bias);
           if (value) { values[3] = __Pyx_Arg_NewRef_FASTCALL(value); kw_args--; }
-          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 741, __pyx_L3_error)
+          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 756, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  4:
         if (kw_args > 0) {
           PyObject* value = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_flat);
           if (value) { values[4] = __Pyx_Arg_NewRef_FASTCALL(value); kw_args--; }
-          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 741, __pyx_L3_error)
+          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 756, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "__init__") < 0)) __PYX_ERR(0, 741, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "__init__") < 0)) __PYX_ERR(0, 756, __pyx_L3_error)
       }
     } else {
       switch (__pyx_nargs) {
         case  5: values[4] = __Pyx_Arg_FASTCALL(__pyx_args, 4);
         CYTHON_FALLTHROUGH;
         case  4: values[3] = __Pyx_Arg_FASTCALL(__pyx_args, 3);
         CYTHON_FALLTHROUGH;
@@ -20021,34 +20586,34 @@
     __pyx_v_matrix_data = ((PyObject*)values[1]);
     __pyx_v_key_bias = ((PyObject*)values[2]);
     __pyx_v_val_bias = ((PyObject*)values[3]);
     __pyx_v_flat = values[4];
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__init__", 0, 2, 5, __pyx_nargs); __PYX_ERR(0, 741, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__init__", 0, 2, 5, __pyx_nargs); __PYX_ERR(0, 756, __pyx_L3_error)
   __pyx_L6_skip:;
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_AddTraceback("Fortuna.FlexCat.__init__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_matrix_data), (&PyDict_Type), 0, "matrix_data", 1))) __PYX_ERR(0, 742, __pyx_L1_error)
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_key_bias), (&PyUnicode_Type), 0, "key_bias", 1))) __PYX_ERR(0, 743, __pyx_L1_error)
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_val_bias), (&PyUnicode_Type), 0, "val_bias", 1))) __PYX_ERR(0, 744, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_matrix_data), (&PyDict_Type), 0, "matrix_data", 1))) __PYX_ERR(0, 757, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_key_bias), (&PyUnicode_Type), 0, "key_bias", 1))) __PYX_ERR(0, 758, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_val_bias), (&PyUnicode_Type), 0, "val_bias", 1))) __PYX_ERR(0, 759, __pyx_L1_error)
   __pyx_r = __pyx_pf_7Fortuna_7FlexCat___init__(__pyx_self, __pyx_v_self, __pyx_v_matrix_data, __pyx_v_key_bias, __pyx_v_val_bias, __pyx_v_flat);
 
-  /* "Fortuna.pyx":741
+  /* "Fortuna.pyx":756
  *                  "double_cycle", "cycle")
  * 
  *     def __init__(self,             # <<<<<<<<<<<<<<
  *                  matrix_data: Dict,
  *                  key_bias: str = "front_linear",
  */
 
@@ -20087,119 +20652,119 @@
   PyObject *__pyx_t_11 = NULL;
   PyObject *__pyx_t_12 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__init__", 1);
 
-  /* "Fortuna.pyx":756
+  /* "Fortuna.pyx":771
  *         @return : Callable Instance
  *         """
  *         self.double_cycle = key_bias == val_bias == "cycle"             # <<<<<<<<<<<<<<
  *         self.matrix_data = matrix_data
  *         self.cat_keys = matrix_data.keys()
  */
-  __pyx_t_1 = (__Pyx_PyUnicode_Equals(__pyx_v_key_bias, __pyx_v_val_bias, Py_EQ)); if (unlikely((__pyx_t_1 < 0))) __PYX_ERR(0, 756, __pyx_L1_error)
+  __pyx_t_1 = (__Pyx_PyUnicode_Equals(__pyx_v_key_bias, __pyx_v_val_bias, Py_EQ)); if (unlikely((__pyx_t_1 < 0))) __PYX_ERR(0, 771, __pyx_L1_error)
   if (__pyx_t_1) {
-    __pyx_t_1 = (__Pyx_PyUnicode_Equals(__pyx_v_val_bias, __pyx_n_u_cycle, Py_EQ)); if (unlikely((__pyx_t_1 < 0))) __PYX_ERR(0, 756, __pyx_L1_error)
+    __pyx_t_1 = (__Pyx_PyUnicode_Equals(__pyx_v_val_bias, __pyx_n_u_cycle, Py_EQ)); if (unlikely((__pyx_t_1 < 0))) __PYX_ERR(0, 771, __pyx_L1_error)
   }
-  __pyx_t_2 = __Pyx_PyBool_FromLong(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 756, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyBool_FromLong(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 771, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_double_cycle, __pyx_t_2) < 0) __PYX_ERR(0, 756, __pyx_L1_error)
+  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_double_cycle, __pyx_t_2) < 0) __PYX_ERR(0, 771, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "Fortuna.pyx":757
+  /* "Fortuna.pyx":772
  *         """
  *         self.double_cycle = key_bias == val_bias == "cycle"
  *         self.matrix_data = matrix_data             # <<<<<<<<<<<<<<
  *         self.cat_keys = matrix_data.keys()
  *         self.random_cat = QuantumMonty(
  */
-  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_matrix_data, __pyx_v_matrix_data) < 0) __PYX_ERR(0, 757, __pyx_L1_error)
+  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_matrix_data, __pyx_v_matrix_data) < 0) __PYX_ERR(0, 772, __pyx_L1_error)
 
-  /* "Fortuna.pyx":758
+  /* "Fortuna.pyx":773
  *         self.double_cycle = key_bias == val_bias == "cycle"
  *         self.matrix_data = matrix_data
  *         self.cat_keys = matrix_data.keys()             # <<<<<<<<<<<<<<
  *         self.random_cat = QuantumMonty(
  *             tuple(self.cat_keys),
  */
-  __pyx_t_2 = __Pyx_PyDict_Keys(__pyx_v_matrix_data); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 758, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyDict_Keys(__pyx_v_matrix_data); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 773, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_cat_keys, __pyx_t_2) < 0) __PYX_ERR(0, 758, __pyx_L1_error)
+  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_cat_keys, __pyx_t_2) < 0) __PYX_ERR(0, 773, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "Fortuna.pyx":759
+  /* "Fortuna.pyx":774
  *         self.matrix_data = matrix_data
  *         self.cat_keys = matrix_data.keys()
  *         self.random_cat = QuantumMonty(             # <<<<<<<<<<<<<<
  *             tuple(self.cat_keys),
  *             flat=False,
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_QuantumMonty); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 759, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_QuantumMonty); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 774, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
 
-  /* "Fortuna.pyx":760
+  /* "Fortuna.pyx":775
  *         self.cat_keys = matrix_data.keys()
  *         self.random_cat = QuantumMonty(
  *             tuple(self.cat_keys),             # <<<<<<<<<<<<<<
  *             flat=False,
  *         ).dispatch(key_bias)
  */
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_cat_keys); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 760, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_cat_keys); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 775, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_5 = __Pyx_PySequence_Tuple(__pyx_t_4); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 760, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PySequence_Tuple(__pyx_t_4); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 775, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "Fortuna.pyx":759
+  /* "Fortuna.pyx":774
  *         self.matrix_data = matrix_data
  *         self.cat_keys = matrix_data.keys()
  *         self.random_cat = QuantumMonty(             # <<<<<<<<<<<<<<
  *             tuple(self.cat_keys),
  *             flat=False,
  */
-  __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 759, __pyx_L1_error)
+  __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 774, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_GIVEREF(__pyx_t_5);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_5)) __PYX_ERR(0, 759, __pyx_L1_error);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_5)) __PYX_ERR(0, 774, __pyx_L1_error);
   __pyx_t_5 = 0;
 
-  /* "Fortuna.pyx":761
+  /* "Fortuna.pyx":776
  *         self.random_cat = QuantumMonty(
  *             tuple(self.cat_keys),
  *             flat=False,             # <<<<<<<<<<<<<<
  *         ).dispatch(key_bias)
  *         self.random_selection = {
  */
-  __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 761, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 776, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_flat, Py_False) < 0) __PYX_ERR(0, 761, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_flat, Py_False) < 0) __PYX_ERR(0, 776, __pyx_L1_error)
 
-  /* "Fortuna.pyx":759
+  /* "Fortuna.pyx":774
  *         self.matrix_data = matrix_data
  *         self.cat_keys = matrix_data.keys()
  *         self.random_cat = QuantumMonty(             # <<<<<<<<<<<<<<
  *             tuple(self.cat_keys),
  *             flat=False,
  */
-  __pyx_t_6 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_4, __pyx_t_5); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 759, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_4, __pyx_t_5); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 774, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
-  /* "Fortuna.pyx":762
+  /* "Fortuna.pyx":777
  *             tuple(self.cat_keys),
  *             flat=False,
  *         ).dispatch(key_bias)             # <<<<<<<<<<<<<<
  *         self.random_selection = {
  *             key: QuantumMonty(
  */
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_dispatch); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 762, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_dispatch); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 777, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   __pyx_t_6 = NULL;
   __pyx_t_7 = 0;
   #if CYTHON_UNPACK_METHODS
   if (likely(PyMethod_Check(__pyx_t_5))) {
     __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_5);
@@ -20212,129 +20777,129 @@
     }
   }
   #endif
   {
     PyObject *__pyx_callargs[2] = {__pyx_t_6, __pyx_v_key_bias};
     __pyx_t_2 = __Pyx_PyObject_FastCall(__pyx_t_5, __pyx_callargs+1-__pyx_t_7, 1+__pyx_t_7);
     __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
-    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 762, __pyx_L1_error)
+    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 777, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   }
 
-  /* "Fortuna.pyx":759
+  /* "Fortuna.pyx":774
  *         self.matrix_data = matrix_data
  *         self.cat_keys = matrix_data.keys()
  *         self.random_cat = QuantumMonty(             # <<<<<<<<<<<<<<
  *             tuple(self.cat_keys),
  *             flat=False,
  */
-  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_random_cat, __pyx_t_2) < 0) __PYX_ERR(0, 759, __pyx_L1_error)
+  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_random_cat, __pyx_t_2) < 0) __PYX_ERR(0, 774, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "Fortuna.pyx":763
+  /* "Fortuna.pyx":778
  *             flat=False,
  *         ).dispatch(key_bias)
  *         self.random_selection = {             # <<<<<<<<<<<<<<
  *             key: QuantumMonty(
  *                 tuple(seq),
  */
   { /* enter inner scope */
-    __pyx_t_2 = PyDict_New(); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 763, __pyx_L5_error)
+    __pyx_t_2 = PyDict_New(); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 778, __pyx_L5_error)
     __Pyx_GOTREF(__pyx_t_2);
 
-    /* "Fortuna.pyx":768
+    /* "Fortuna.pyx":783
  *                 flat=flat,
  *             ).dispatch(val_bias)
  *             for key, seq in matrix_data.items()             # <<<<<<<<<<<<<<
  *         }
  *         cycle_source = []
  */
     __pyx_t_8 = 0;
-    __pyx_t_6 = __Pyx_dict_iterator(__pyx_v_matrix_data, 1, __pyx_n_s_items, (&__pyx_t_9), (&__pyx_t_7)); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 768, __pyx_L5_error)
+    __pyx_t_6 = __Pyx_dict_iterator(__pyx_v_matrix_data, 1, __pyx_n_s_items, (&__pyx_t_9), (&__pyx_t_7)); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 783, __pyx_L5_error)
     __Pyx_GOTREF(__pyx_t_6);
     __Pyx_XDECREF(__pyx_t_5);
     __pyx_t_5 = __pyx_t_6;
     __pyx_t_6 = 0;
     while (1) {
       __pyx_t_10 = __Pyx_dict_iter_next(__pyx_t_5, __pyx_t_9, &__pyx_t_8, &__pyx_t_6, &__pyx_t_4, NULL, __pyx_t_7);
       if (unlikely(__pyx_t_10 == 0)) break;
-      if (unlikely(__pyx_t_10 == -1)) __PYX_ERR(0, 768, __pyx_L5_error)
+      if (unlikely(__pyx_t_10 == -1)) __PYX_ERR(0, 783, __pyx_L5_error)
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_4);
       __Pyx_XDECREF_SET(__pyx_7genexpr__pyx_v_key, __pyx_t_6);
       __pyx_t_6 = 0;
       __Pyx_XDECREF_SET(__pyx_7genexpr__pyx_v_seq, __pyx_t_4);
       __pyx_t_4 = 0;
 
-      /* "Fortuna.pyx":764
+      /* "Fortuna.pyx":779
  *         ).dispatch(key_bias)
  *         self.random_selection = {
  *             key: QuantumMonty(             # <<<<<<<<<<<<<<
  *                 tuple(seq),
  *                 flat=flat,
  */
-      __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_QuantumMonty); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 764, __pyx_L5_error)
+      __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_QuantumMonty); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 779, __pyx_L5_error)
       __Pyx_GOTREF(__pyx_t_6);
 
-      /* "Fortuna.pyx":765
+      /* "Fortuna.pyx":780
  *         self.random_selection = {
  *             key: QuantumMonty(
  *                 tuple(seq),             # <<<<<<<<<<<<<<
  *                 flat=flat,
  *             ).dispatch(val_bias)
  */
-      __pyx_t_3 = __Pyx_PySequence_Tuple(__pyx_7genexpr__pyx_v_seq); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 765, __pyx_L5_error)
+      __pyx_t_3 = __Pyx_PySequence_Tuple(__pyx_7genexpr__pyx_v_seq); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 780, __pyx_L5_error)
       __Pyx_GOTREF(__pyx_t_3);
 
-      /* "Fortuna.pyx":764
+      /* "Fortuna.pyx":779
  *         ).dispatch(key_bias)
  *         self.random_selection = {
  *             key: QuantumMonty(             # <<<<<<<<<<<<<<
  *                 tuple(seq),
  *                 flat=flat,
  */
-      __pyx_t_11 = PyTuple_New(1); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 764, __pyx_L5_error)
+      __pyx_t_11 = PyTuple_New(1); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 779, __pyx_L5_error)
       __Pyx_GOTREF(__pyx_t_11);
       __Pyx_GIVEREF(__pyx_t_3);
-      if (__Pyx_PyTuple_SET_ITEM(__pyx_t_11, 0, __pyx_t_3)) __PYX_ERR(0, 764, __pyx_L5_error);
+      if (__Pyx_PyTuple_SET_ITEM(__pyx_t_11, 0, __pyx_t_3)) __PYX_ERR(0, 779, __pyx_L5_error);
       __pyx_t_3 = 0;
 
-      /* "Fortuna.pyx":766
+      /* "Fortuna.pyx":781
  *             key: QuantumMonty(
  *                 tuple(seq),
  *                 flat=flat,             # <<<<<<<<<<<<<<
  *             ).dispatch(val_bias)
  *             for key, seq in matrix_data.items()
  */
-      __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 766, __pyx_L5_error)
+      __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 781, __pyx_L5_error)
       __Pyx_GOTREF(__pyx_t_3);
-      if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_flat, __pyx_v_flat) < 0) __PYX_ERR(0, 766, __pyx_L5_error)
+      if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_flat, __pyx_v_flat) < 0) __PYX_ERR(0, 781, __pyx_L5_error)
 
-      /* "Fortuna.pyx":764
+      /* "Fortuna.pyx":779
  *         ).dispatch(key_bias)
  *         self.random_selection = {
  *             key: QuantumMonty(             # <<<<<<<<<<<<<<
  *                 tuple(seq),
  *                 flat=flat,
  */
-      __pyx_t_12 = __Pyx_PyObject_Call(__pyx_t_6, __pyx_t_11, __pyx_t_3); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 764, __pyx_L5_error)
+      __pyx_t_12 = __Pyx_PyObject_Call(__pyx_t_6, __pyx_t_11, __pyx_t_3); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 779, __pyx_L5_error)
       __Pyx_GOTREF(__pyx_t_12);
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
       __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-      /* "Fortuna.pyx":767
+      /* "Fortuna.pyx":782
  *                 tuple(seq),
  *                 flat=flat,
  *             ).dispatch(val_bias)             # <<<<<<<<<<<<<<
  *             for key, seq in matrix_data.items()
  *         }
  */
-      __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_12, __pyx_n_s_dispatch); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 767, __pyx_L5_error)
+      __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_12, __pyx_n_s_dispatch); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 782, __pyx_L5_error)
       __Pyx_GOTREF(__pyx_t_3);
       __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
       __pyx_t_12 = NULL;
       __pyx_t_10 = 0;
       #if CYTHON_UNPACK_METHODS
       if (likely(PyMethod_Check(__pyx_t_3))) {
         __pyx_t_12 = PyMethod_GET_SELF(__pyx_t_3);
@@ -20347,97 +20912,97 @@
         }
       }
       #endif
       {
         PyObject *__pyx_callargs[2] = {__pyx_t_12, __pyx_v_val_bias};
         __pyx_t_4 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_10, 1+__pyx_t_10);
         __Pyx_XDECREF(__pyx_t_12); __pyx_t_12 = 0;
-        if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 767, __pyx_L5_error)
+        if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 782, __pyx_L5_error)
         __Pyx_GOTREF(__pyx_t_4);
         __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
       }
-      if (unlikely(PyDict_SetItem(__pyx_t_2, (PyObject*)__pyx_7genexpr__pyx_v_key, (PyObject*)__pyx_t_4))) __PYX_ERR(0, 764, __pyx_L5_error)
+      if (unlikely(PyDict_SetItem(__pyx_t_2, (PyObject*)__pyx_7genexpr__pyx_v_key, (PyObject*)__pyx_t_4))) __PYX_ERR(0, 779, __pyx_L5_error)
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     }
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_XDECREF(__pyx_7genexpr__pyx_v_key); __pyx_7genexpr__pyx_v_key = 0;
     __Pyx_XDECREF(__pyx_7genexpr__pyx_v_seq); __pyx_7genexpr__pyx_v_seq = 0;
     goto __pyx_L8_exit_scope;
     __pyx_L5_error:;
     __Pyx_XDECREF(__pyx_7genexpr__pyx_v_key); __pyx_7genexpr__pyx_v_key = 0;
     __Pyx_XDECREF(__pyx_7genexpr__pyx_v_seq); __pyx_7genexpr__pyx_v_seq = 0;
     goto __pyx_L1_error;
     __pyx_L8_exit_scope:;
   } /* exit inner scope */
 
-  /* "Fortuna.pyx":763
+  /* "Fortuna.pyx":778
  *             flat=False,
  *         ).dispatch(key_bias)
  *         self.random_selection = {             # <<<<<<<<<<<<<<
  *             key: QuantumMonty(
  *                 tuple(seq),
  */
-  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_random_selection, __pyx_t_2) < 0) __PYX_ERR(0, 763, __pyx_L1_error)
+  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_random_selection, __pyx_t_2) < 0) __PYX_ERR(0, 778, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "Fortuna.pyx":770
+  /* "Fortuna.pyx":785
  *             for key, seq in matrix_data.items()
  *         }
  *         cycle_source = []             # <<<<<<<<<<<<<<
  *         for seq in matrix_data.values():
  *             cycle_source += seq
  */
-  __pyx_t_2 = PyList_New(0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 770, __pyx_L1_error)
+  __pyx_t_2 = PyList_New(0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 785, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_v_cycle_source = __pyx_t_2;
   __pyx_t_2 = 0;
 
-  /* "Fortuna.pyx":771
+  /* "Fortuna.pyx":786
  *         }
  *         cycle_source = []
  *         for seq in matrix_data.values():             # <<<<<<<<<<<<<<
  *             cycle_source += seq
  *         self.cycle = cycle(cycle_source)
  */
   __pyx_t_9 = 0;
-  __pyx_t_5 = __Pyx_dict_iterator(__pyx_v_matrix_data, 1, __pyx_n_s_values, (&__pyx_t_8), (&__pyx_t_7)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 771, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_dict_iterator(__pyx_v_matrix_data, 1, __pyx_n_s_values, (&__pyx_t_8), (&__pyx_t_7)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 786, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_XDECREF(__pyx_t_2);
   __pyx_t_2 = __pyx_t_5;
   __pyx_t_5 = 0;
   while (1) {
     __pyx_t_10 = __Pyx_dict_iter_next(__pyx_t_2, __pyx_t_8, &__pyx_t_9, NULL, &__pyx_t_5, NULL, __pyx_t_7);
     if (unlikely(__pyx_t_10 == 0)) break;
-    if (unlikely(__pyx_t_10 == -1)) __PYX_ERR(0, 771, __pyx_L1_error)
+    if (unlikely(__pyx_t_10 == -1)) __PYX_ERR(0, 786, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_XDECREF_SET(__pyx_v_seq, __pyx_t_5);
     __pyx_t_5 = 0;
 
-    /* "Fortuna.pyx":772
+    /* "Fortuna.pyx":787
  *         cycle_source = []
  *         for seq in matrix_data.values():
  *             cycle_source += seq             # <<<<<<<<<<<<<<
  *         self.cycle = cycle(cycle_source)
  * 
  */
-    __pyx_t_5 = PyNumber_InPlaceAdd(__pyx_v_cycle_source, __pyx_v_seq); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 772, __pyx_L1_error)
+    __pyx_t_5 = PyNumber_InPlaceAdd(__pyx_v_cycle_source, __pyx_v_seq); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 787, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_DECREF_SET(__pyx_v_cycle_source, __pyx_t_5);
     __pyx_t_5 = 0;
   }
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "Fortuna.pyx":773
+  /* "Fortuna.pyx":788
  *         for seq in matrix_data.values():
  *             cycle_source += seq
  *         self.cycle = cycle(cycle_source)             # <<<<<<<<<<<<<<
  * 
  *     def __call__(self, cat_key=None, *args, **kwargs):
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_cycle); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 773, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_cycle); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 788, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __pyx_t_4 = NULL;
   __pyx_t_7 = 0;
   #if CYTHON_UNPACK_METHODS
   if (unlikely(PyMethod_Check(__pyx_t_5))) {
     __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_5);
     if (likely(__pyx_t_4)) {
@@ -20449,22 +21014,22 @@
     }
   }
   #endif
   {
     PyObject *__pyx_callargs[2] = {__pyx_t_4, __pyx_v_cycle_source};
     __pyx_t_2 = __Pyx_PyObject_FastCall(__pyx_t_5, __pyx_callargs+1-__pyx_t_7, 1+__pyx_t_7);
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 773, __pyx_L1_error)
+    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 788, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   }
-  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_cycle, __pyx_t_2) < 0) __PYX_ERR(0, 773, __pyx_L1_error)
+  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_cycle, __pyx_t_2) < 0) __PYX_ERR(0, 788, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "Fortuna.pyx":741
+  /* "Fortuna.pyx":756
  *                  "double_cycle", "cycle")
  * 
  *     def __init__(self,             # <<<<<<<<<<<<<<
  *                  matrix_data: Dict,
  *                  key_bias: str = "front_linear",
  */
 
@@ -20487,15 +21052,15 @@
   __Pyx_XDECREF(__pyx_7genexpr__pyx_v_key);
   __Pyx_XDECREF(__pyx_7genexpr__pyx_v_seq);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "Fortuna.pyx":775
+/* "Fortuna.pyx":790
  *         self.cycle = cycle(cycle_source)
  * 
  *     def __call__(self, cat_key=None, *args, **kwargs):             # <<<<<<<<<<<<<<
  *         """
  *         @param cat_key : Optional String. Default is None.
  */
 
@@ -20564,28 +21129,28 @@
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_self)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 775, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 790, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (kw_args > 0) {
           PyObject* value = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_cat_key);
           if (value) { values[1] = __Pyx_Arg_NewRef_FASTCALL(value); kw_args--; }
-          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 775, __pyx_L3_error)
+          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 790, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
         const Py_ssize_t used_pos_args = (kwd_pos_args < 2) ? kwd_pos_args : 2;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, __pyx_v_kwargs, values + 0, used_pos_args, "__call__") < 0)) __PYX_ERR(0, 775, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, __pyx_v_kwargs, values + 0, used_pos_args, "__call__") < 0)) __PYX_ERR(0, 790, __pyx_L3_error)
       }
     } else {
       switch (__pyx_nargs) {
         default:
         case  2: values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
         CYTHON_FALLTHROUGH;
         case  1: values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
@@ -20595,15 +21160,15 @@
       }
     }
     __pyx_v_self = values[0];
     __pyx_v_cat_key = values[1];
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__call__", 0, 1, 2, __pyx_nargs); __PYX_ERR(0, 775, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__call__", 0, 1, 2, __pyx_nargs); __PYX_ERR(0, 790, __pyx_L3_error)
   __pyx_L6_skip:;
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
@@ -20644,87 +21209,87 @@
   PyObject *__pyx_t_7 = NULL;
   int __pyx_t_8;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__call__", 1);
 
-  /* "Fortuna.pyx":784
+  /* "Fortuna.pyx":799
  *             from a random sequence generated with key_bias.
  *         """
  *         if not cat_key and self.double_cycle:             # <<<<<<<<<<<<<<
  *             return next(self.cycle)
  *         monty = self.random_selection
  */
-  __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_v_cat_key); if (unlikely((__pyx_t_2 < 0))) __PYX_ERR(0, 784, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_v_cat_key); if (unlikely((__pyx_t_2 < 0))) __PYX_ERR(0, 799, __pyx_L1_error)
   __pyx_t_3 = (!__pyx_t_2);
   if (__pyx_t_3) {
   } else {
     __pyx_t_1 = __pyx_t_3;
     goto __pyx_L4_bool_binop_done;
   }
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_double_cycle); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 784, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_double_cycle); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 799, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_3 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely((__pyx_t_3 < 0))) __PYX_ERR(0, 784, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely((__pyx_t_3 < 0))) __PYX_ERR(0, 799, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __pyx_t_1 = __pyx_t_3;
   __pyx_L4_bool_binop_done:;
   if (__pyx_t_1) {
 
-    /* "Fortuna.pyx":785
+    /* "Fortuna.pyx":800
  *         """
  *         if not cat_key and self.double_cycle:
  *             return next(self.cycle)             # <<<<<<<<<<<<<<
  *         monty = self.random_selection
  *         key = cat_key if cat_key is not None else self.random_cat()
  */
     __Pyx_XDECREF(__pyx_r);
-    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_cycle); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 785, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_cycle); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 800, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_5 = __Pyx_PyIter_Next(__pyx_t_4); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 785, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyIter_Next(__pyx_t_4); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 800, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __pyx_r = __pyx_t_5;
     __pyx_t_5 = 0;
     goto __pyx_L0;
 
-    /* "Fortuna.pyx":784
+    /* "Fortuna.pyx":799
  *             from a random sequence generated with key_bias.
  *         """
  *         if not cat_key and self.double_cycle:             # <<<<<<<<<<<<<<
  *             return next(self.cycle)
  *         monty = self.random_selection
  */
   }
 
-  /* "Fortuna.pyx":786
+  /* "Fortuna.pyx":801
  *         if not cat_key and self.double_cycle:
  *             return next(self.cycle)
  *         monty = self.random_selection             # <<<<<<<<<<<<<<
  *         key = cat_key if cat_key is not None else self.random_cat()
  *         return monty[key](*args, **kwargs)
  */
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_random_selection); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 786, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_random_selection); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 801, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __pyx_v_monty = __pyx_t_5;
   __pyx_t_5 = 0;
 
-  /* "Fortuna.pyx":787
+  /* "Fortuna.pyx":802
  *             return next(self.cycle)
  *         monty = self.random_selection
  *         key = cat_key if cat_key is not None else self.random_cat()             # <<<<<<<<<<<<<<
  *         return monty[key](*args, **kwargs)
  * 
  */
   __pyx_t_1 = (__pyx_v_cat_key != Py_None);
   if (__pyx_t_1) {
     __Pyx_INCREF(__pyx_v_cat_key);
     __pyx_t_5 = __pyx_v_cat_key;
   } else {
-    __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_random_cat); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 787, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_random_cat); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 802, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __pyx_t_7 = NULL;
     __pyx_t_8 = 0;
     #if CYTHON_UNPACK_METHODS
     if (likely(PyMethod_Check(__pyx_t_6))) {
       __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_6);
       if (likely(__pyx_t_7)) {
@@ -20736,45 +21301,45 @@
       }
     }
     #endif
     {
       PyObject *__pyx_callargs[2] = {__pyx_t_7, NULL};
       __pyx_t_4 = __Pyx_PyObject_FastCall(__pyx_t_6, __pyx_callargs+1-__pyx_t_8, 0+__pyx_t_8);
       __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
-      if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 787, __pyx_L1_error)
+      if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 802, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     }
     __pyx_t_5 = __pyx_t_4;
     __pyx_t_4 = 0;
   }
   __pyx_v_key = __pyx_t_5;
   __pyx_t_5 = 0;
 
-  /* "Fortuna.pyx":788
+  /* "Fortuna.pyx":803
  *         monty = self.random_selection
  *         key = cat_key if cat_key is not None else self.random_cat()
  *         return monty[key](*args, **kwargs)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_5 = __Pyx_PyObject_GetItem(__pyx_v_monty, __pyx_v_key); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 788, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_GetItem(__pyx_v_monty, __pyx_v_key); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 803, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_4 = PyDict_Copy(__pyx_v_kwargs); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 788, __pyx_L1_error)
+  __pyx_t_4 = PyDict_Copy(__pyx_v_kwargs); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 803, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_6 = __Pyx_PyObject_Call(__pyx_t_5, __pyx_v_args, __pyx_t_4); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 788, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_Call(__pyx_t_5, __pyx_v_args, __pyx_t_4); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 803, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __pyx_r = __pyx_t_6;
   __pyx_t_6 = 0;
   goto __pyx_L0;
 
-  /* "Fortuna.pyx":775
+  /* "Fortuna.pyx":790
  *         self.cycle = cycle(cycle_source)
  * 
  *     def __call__(self, cat_key=None, *args, **kwargs):             # <<<<<<<<<<<<<<
  *         """
  *         @param cat_key : Optional String. Default is None.
  */
 
@@ -20790,15 +21355,15 @@
   __Pyx_XDECREF(__pyx_v_monty);
   __Pyx_XDECREF(__pyx_v_key);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "Fortuna.pyx":809
+/* "Fortuna.pyx":824
  *     __slots__ = ("flat", "max_weight", "data")
  * 
  *     def __call__(self, *args, **kwargs):             # <<<<<<<<<<<<<<
  *         """
  *         @param *args, **kwargs : Optional arguments
  */
 
@@ -20863,32 +21428,32 @@
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_self)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 809, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 824, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
         const Py_ssize_t used_pos_args = (kwd_pos_args < 1) ? kwd_pos_args : 1;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, __pyx_v_kwargs, values + 0, used_pos_args, "__call__") < 0)) __PYX_ERR(0, 809, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, __pyx_v_kwargs, values + 0, used_pos_args, "__call__") < 0)) __PYX_ERR(0, 824, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs < 1)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
     }
     __pyx_v_self = values[0];
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__call__", 0, 1, 1, __pyx_nargs); __PYX_ERR(0, 809, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__call__", 0, 1, 1, __pyx_nargs); __PYX_ERR(0, 824, __pyx_L3_error)
   __pyx_L6_skip:;
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
@@ -20933,212 +21498,212 @@
   int __pyx_t_10;
   PyObject *__pyx_t_11 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__call__", 1);
 
-  /* "Fortuna.pyx":816
+  /* "Fortuna.pyx":831
  *             distribution based on the weights of the values.
  *         """
  *         rand = _random_below(self.max_weight)             # <<<<<<<<<<<<<<
  *         for weight, value in self.data:
  *             if weight > rand:
  */
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_max_weight); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 816, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_max_weight); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 831, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyInt_As_PY_LONG_LONG(__pyx_t_1); if (unlikely((__pyx_t_2 == (PY_LONG_LONG)-1) && PyErr_Occurred())) __PYX_ERR(0, 816, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_As_PY_LONG_LONG(__pyx_t_1); if (unlikely((__pyx_t_2 == (PY_LONG_LONG)-1) && PyErr_Occurred())) __PYX_ERR(0, 831, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_v_rand = Storm::GetInt::random_below(__pyx_t_2);
 
-  /* "Fortuna.pyx":817
+  /* "Fortuna.pyx":832
  *         """
  *         rand = _random_below(self.max_weight)
  *         for weight, value in self.data:             # <<<<<<<<<<<<<<
  *             if weight > rand:
  *                 return flatten(value, *args, flat=self.flat, **kwargs)
  */
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_data); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 817, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_data); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 832, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (likely(PyList_CheckExact(__pyx_t_1)) || PyTuple_CheckExact(__pyx_t_1)) {
     __pyx_t_3 = __pyx_t_1; __Pyx_INCREF(__pyx_t_3);
     __pyx_t_4 = 0;
     __pyx_t_5 = NULL;
   } else {
-    __pyx_t_4 = -1; __pyx_t_3 = PyObject_GetIter(__pyx_t_1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 817, __pyx_L1_error)
+    __pyx_t_4 = -1; __pyx_t_3 = PyObject_GetIter(__pyx_t_1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 832, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_5 = __Pyx_PyObject_GetIterNextFunc(__pyx_t_3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 817, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyObject_GetIterNextFunc(__pyx_t_3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 832, __pyx_L1_error)
   }
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   for (;;) {
     if (likely(!__pyx_t_5)) {
       if (likely(PyList_CheckExact(__pyx_t_3))) {
         {
           Py_ssize_t __pyx_temp = __Pyx_PyList_GET_SIZE(__pyx_t_3);
           #if !CYTHON_ASSUME_SAFE_MACROS
-          if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 817, __pyx_L1_error)
+          if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 832, __pyx_L1_error)
           #endif
           if (__pyx_t_4 >= __pyx_temp) break;
         }
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_1 = PyList_GET_ITEM(__pyx_t_3, __pyx_t_4); __Pyx_INCREF(__pyx_t_1); __pyx_t_4++; if (unlikely((0 < 0))) __PYX_ERR(0, 817, __pyx_L1_error)
+        __pyx_t_1 = PyList_GET_ITEM(__pyx_t_3, __pyx_t_4); __Pyx_INCREF(__pyx_t_1); __pyx_t_4++; if (unlikely((0 < 0))) __PYX_ERR(0, 832, __pyx_L1_error)
         #else
-        __pyx_t_1 = __Pyx_PySequence_ITEM(__pyx_t_3, __pyx_t_4); __pyx_t_4++; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 817, __pyx_L1_error)
+        __pyx_t_1 = __Pyx_PySequence_ITEM(__pyx_t_3, __pyx_t_4); __pyx_t_4++; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 832, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_1);
         #endif
       } else {
         {
           Py_ssize_t __pyx_temp = __Pyx_PyTuple_GET_SIZE(__pyx_t_3);
           #if !CYTHON_ASSUME_SAFE_MACROS
-          if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 817, __pyx_L1_error)
+          if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 832, __pyx_L1_error)
           #endif
           if (__pyx_t_4 >= __pyx_temp) break;
         }
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_1 = PyTuple_GET_ITEM(__pyx_t_3, __pyx_t_4); __Pyx_INCREF(__pyx_t_1); __pyx_t_4++; if (unlikely((0 < 0))) __PYX_ERR(0, 817, __pyx_L1_error)
+        __pyx_t_1 = PyTuple_GET_ITEM(__pyx_t_3, __pyx_t_4); __Pyx_INCREF(__pyx_t_1); __pyx_t_4++; if (unlikely((0 < 0))) __PYX_ERR(0, 832, __pyx_L1_error)
         #else
-        __pyx_t_1 = __Pyx_PySequence_ITEM(__pyx_t_3, __pyx_t_4); __pyx_t_4++; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 817, __pyx_L1_error)
+        __pyx_t_1 = __Pyx_PySequence_ITEM(__pyx_t_3, __pyx_t_4); __pyx_t_4++; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 832, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_1);
         #endif
       }
     } else {
       __pyx_t_1 = __pyx_t_5(__pyx_t_3);
       if (unlikely(!__pyx_t_1)) {
         PyObject* exc_type = PyErr_Occurred();
         if (exc_type) {
           if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-          else __PYX_ERR(0, 817, __pyx_L1_error)
+          else __PYX_ERR(0, 832, __pyx_L1_error)
         }
         break;
       }
       __Pyx_GOTREF(__pyx_t_1);
     }
     if ((likely(PyTuple_CheckExact(__pyx_t_1))) || (PyList_CheckExact(__pyx_t_1))) {
       PyObject* sequence = __pyx_t_1;
       Py_ssize_t size = __Pyx_PySequence_SIZE(sequence);
       if (unlikely(size != 2)) {
         if (size > 2) __Pyx_RaiseTooManyValuesError(2);
         else if (size >= 0) __Pyx_RaiseNeedMoreValuesError(size);
-        __PYX_ERR(0, 817, __pyx_L1_error)
+        __PYX_ERR(0, 832, __pyx_L1_error)
       }
       #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
       if (likely(PyTuple_CheckExact(sequence))) {
         __pyx_t_6 = PyTuple_GET_ITEM(sequence, 0); 
         __pyx_t_7 = PyTuple_GET_ITEM(sequence, 1); 
       } else {
         __pyx_t_6 = PyList_GET_ITEM(sequence, 0); 
         __pyx_t_7 = PyList_GET_ITEM(sequence, 1); 
       }
       __Pyx_INCREF(__pyx_t_6);
       __Pyx_INCREF(__pyx_t_7);
       #else
-      __pyx_t_6 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 817, __pyx_L1_error)
+      __pyx_t_6 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 832, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_6);
-      __pyx_t_7 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 817, __pyx_L1_error)
+      __pyx_t_7 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 832, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_7);
       #endif
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     } else {
       Py_ssize_t index = -1;
-      __pyx_t_8 = PyObject_GetIter(__pyx_t_1); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 817, __pyx_L1_error)
+      __pyx_t_8 = PyObject_GetIter(__pyx_t_1); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 832, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       __pyx_t_9 = __Pyx_PyObject_GetIterNextFunc(__pyx_t_8);
       index = 0; __pyx_t_6 = __pyx_t_9(__pyx_t_8); if (unlikely(!__pyx_t_6)) goto __pyx_L5_unpacking_failed;
       __Pyx_GOTREF(__pyx_t_6);
       index = 1; __pyx_t_7 = __pyx_t_9(__pyx_t_8); if (unlikely(!__pyx_t_7)) goto __pyx_L5_unpacking_failed;
       __Pyx_GOTREF(__pyx_t_7);
-      if (__Pyx_IternextUnpackEndCheck(__pyx_t_9(__pyx_t_8), 2) < 0) __PYX_ERR(0, 817, __pyx_L1_error)
+      if (__Pyx_IternextUnpackEndCheck(__pyx_t_9(__pyx_t_8), 2) < 0) __PYX_ERR(0, 832, __pyx_L1_error)
       __pyx_t_9 = NULL;
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       goto __pyx_L6_unpacking_done;
       __pyx_L5_unpacking_failed:;
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __pyx_t_9 = NULL;
       if (__Pyx_IterFinish() == 0) __Pyx_RaiseNeedMoreValuesError(index);
-      __PYX_ERR(0, 817, __pyx_L1_error)
+      __PYX_ERR(0, 832, __pyx_L1_error)
       __pyx_L6_unpacking_done:;
     }
     __Pyx_XDECREF_SET(__pyx_v_weight, __pyx_t_6);
     __pyx_t_6 = 0;
     __Pyx_XDECREF_SET(__pyx_v_value, __pyx_t_7);
     __pyx_t_7 = 0;
 
-    /* "Fortuna.pyx":818
+    /* "Fortuna.pyx":833
  *         rand = _random_below(self.max_weight)
  *         for weight, value in self.data:
  *             if weight > rand:             # <<<<<<<<<<<<<<
  *                 return flatten(value, *args, flat=self.flat, **kwargs)
  * 
  */
-    __pyx_t_1 = __Pyx_PyInt_From_PY_LONG_LONG(__pyx_v_rand); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 818, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyInt_From_PY_LONG_LONG(__pyx_v_rand); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 833, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_7 = PyObject_RichCompare(__pyx_v_weight, __pyx_t_1, Py_GT); __Pyx_XGOTREF(__pyx_t_7); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 818, __pyx_L1_error)
+    __pyx_t_7 = PyObject_RichCompare(__pyx_v_weight, __pyx_t_1, Py_GT); __Pyx_XGOTREF(__pyx_t_7); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 833, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __pyx_t_10 = __Pyx_PyObject_IsTrue(__pyx_t_7); if (unlikely((__pyx_t_10 < 0))) __PYX_ERR(0, 818, __pyx_L1_error)
+    __pyx_t_10 = __Pyx_PyObject_IsTrue(__pyx_t_7); if (unlikely((__pyx_t_10 < 0))) __PYX_ERR(0, 833, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
     if (__pyx_t_10) {
 
-      /* "Fortuna.pyx":819
+      /* "Fortuna.pyx":834
  *         for weight, value in self.data:
  *             if weight > rand:
  *                 return flatten(value, *args, flat=self.flat, **kwargs)             # <<<<<<<<<<<<<<
  * 
  * 
  */
       __Pyx_XDECREF(__pyx_r);
-      __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_flatten); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 819, __pyx_L1_error)
+      __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_flatten); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 834, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_7);
-      __pyx_t_1 = PyTuple_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 819, __pyx_L1_error)
+      __pyx_t_1 = PyTuple_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 834, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_INCREF(__pyx_v_value);
       __Pyx_GIVEREF(__pyx_v_value);
-      if (__Pyx_PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_v_value)) __PYX_ERR(0, 819, __pyx_L1_error);
-      __pyx_t_6 = PyNumber_Add(__pyx_t_1, __pyx_v_args); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 819, __pyx_L1_error)
+      if (__Pyx_PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_v_value)) __PYX_ERR(0, 834, __pyx_L1_error);
+      __pyx_t_6 = PyNumber_Add(__pyx_t_1, __pyx_v_args); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 834, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-      __pyx_t_8 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 819, __pyx_L1_error)
+      __pyx_t_8 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 834, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_8);
-      __pyx_t_11 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_flat); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 819, __pyx_L1_error)
+      __pyx_t_11 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_flat); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 834, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_11);
-      if (PyDict_SetItem(__pyx_t_8, __pyx_n_s_flat, __pyx_t_11) < 0) __PYX_ERR(0, 819, __pyx_L1_error)
+      if (PyDict_SetItem(__pyx_t_8, __pyx_n_s_flat, __pyx_t_11) < 0) __PYX_ERR(0, 834, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
       __pyx_t_1 = __pyx_t_8;
       __pyx_t_8 = 0;
-      if (__Pyx_MergeKeywords(__pyx_t_1, __pyx_v_kwargs) < 0) __PYX_ERR(0, 819, __pyx_L1_error)
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_t_7, __pyx_t_6, __pyx_t_1); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 819, __pyx_L1_error)
+      if (__Pyx_MergeKeywords(__pyx_t_1, __pyx_v_kwargs) < 0) __PYX_ERR(0, 834, __pyx_L1_error)
+      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_t_7, __pyx_t_6, __pyx_t_1); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 834, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       __pyx_r = __pyx_t_8;
       __pyx_t_8 = 0;
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
       goto __pyx_L0;
 
-      /* "Fortuna.pyx":818
+      /* "Fortuna.pyx":833
  *         rand = _random_below(self.max_weight)
  *         for weight, value in self.data:
  *             if weight > rand:             # <<<<<<<<<<<<<<
  *                 return flatten(value, *args, flat=self.flat, **kwargs)
  * 
  */
     }
 
-    /* "Fortuna.pyx":817
+    /* "Fortuna.pyx":832
  *         """
  *         rand = _random_below(self.max_weight)
  *         for weight, value in self.data:             # <<<<<<<<<<<<<<
  *             if weight > rand:
  *                 return flatten(value, *args, flat=self.flat, **kwargs)
  */
   }
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "Fortuna.pyx":809
+  /* "Fortuna.pyx":824
  *     __slots__ = ("flat", "max_weight", "data")
  * 
  *     def __call__(self, *args, **kwargs):             # <<<<<<<<<<<<<<
  *         """
  *         @param *args, **kwargs : Optional arguments
  */
 
@@ -21158,15 +21723,15 @@
   __Pyx_XDECREF(__pyx_v_weight);
   __Pyx_XDECREF(__pyx_v_value);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "Fortuna.pyx":826
+/* "Fortuna.pyx":841
  *     __slots__ = ("flat", "max_weight", "data")
  * 
  *     def __init__(self,             # <<<<<<<<<<<<<<
  *                  weighted_table: Iterable,
  *                  flat: bool = True):
  */
 
@@ -21208,15 +21773,15 @@
   __pyx_nargs = PyTuple_Size(__pyx_args); if (unlikely(__pyx_nargs < 0)) return NULL;
   #endif
   #endif
   __pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
   {
     PyObject **__pyx_pyargnames[] = {&__pyx_n_s_self,&__pyx_n_s_weighted_table,&__pyx_n_s_flat,0};
 
-    /* "Fortuna.pyx":828
+    /* "Fortuna.pyx":843
  *     def __init__(self,
  *                  weighted_table: Iterable,
  *                  flat: bool = True):             # <<<<<<<<<<<<<<
  *         """
  *         @param weighted_table : Table of weighted pairs.
  */
     values[2] = __Pyx_Arg_NewRef_FASTCALL(((PyObject *)((PyObject *)Py_True)));
@@ -21235,37 +21800,37 @@
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_self)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 826, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 841, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_weighted_table)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[1]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 826, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 841, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("__init__", 0, 2, 3, 1); __PYX_ERR(0, 826, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__init__", 0, 2, 3, 1); __PYX_ERR(0, 841, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (kw_args > 0) {
           PyObject* value = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_flat);
           if (value) { values[2] = __Pyx_Arg_NewRef_FASTCALL(value); kw_args--; }
-          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 826, __pyx_L3_error)
+          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 841, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "__init__") < 0)) __PYX_ERR(0, 826, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "__init__") < 0)) __PYX_ERR(0, 841, __pyx_L3_error)
       }
     } else {
       switch (__pyx_nargs) {
         case  3: values[2] = __Pyx_Arg_FASTCALL(__pyx_args, 2);
         CYTHON_FALLTHROUGH;
         case  2: values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
         values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
@@ -21275,15 +21840,15 @@
     }
     __pyx_v_self = values[0];
     __pyx_v_weighted_table = values[1];
     __pyx_v_flat = values[2];
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__init__", 0, 2, 3, __pyx_nargs); __PYX_ERR(0, 826, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__init__", 0, 2, 3, __pyx_nargs); __PYX_ERR(0, 841, __pyx_L3_error)
   __pyx_L6_skip:;
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
@@ -21291,15 +21856,15 @@
   }
   __Pyx_AddTraceback("Fortuna.RelativeWeightedChoice.__init__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_7Fortuna_22RelativeWeightedChoice___init__(__pyx_self, __pyx_v_self, __pyx_v_weighted_table, __pyx_v_flat);
 
-  /* "Fortuna.pyx":826
+  /* "Fortuna.pyx":841
  *     __slots__ = ("flat", "max_weight", "data")
  * 
  *     def __init__(self,             # <<<<<<<<<<<<<<
  *                  weighted_table: Iterable,
  *                  flat: bool = True):
  */
 
@@ -21310,15 +21875,15 @@
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "Fortuna.pyx":839
+/* "Fortuna.pyx":854
  *         optimized_data = sorted(
  *             [list(itm) for itm in weighted_table],
  *             key=lambda x: x[0], reverse=True)             # <<<<<<<<<<<<<<
  *         cum_weight = 0
  *         for w_pair in optimized_data:
  */
 
@@ -21371,31 +21936,31 @@
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_x)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 839, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 854, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "lambda") < 0)) __PYX_ERR(0, 839, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "lambda") < 0)) __PYX_ERR(0, 854, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs != 1)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
     }
     __pyx_v_x = values[0];
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("lambda", 1, 1, 1, __pyx_nargs); __PYX_ERR(0, 839, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("lambda", 1, 1, 1, __pyx_nargs); __PYX_ERR(0, 854, __pyx_L3_error)
   __pyx_L6_skip:;
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
@@ -21423,15 +21988,15 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("lambda", 1);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_GetItemInt(__pyx_v_x, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 839, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_GetItemInt(__pyx_v_x, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 854, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -21441,15 +22006,15 @@
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 static PyObject *__pyx_gb_7Fortuna_22RelativeWeightedChoice_8__init___3generator(__pyx_CoroutineObject *__pyx_generator, CYTHON_UNUSED PyThreadState *__pyx_tstate, PyObject *__pyx_sent_value); /* proto */
 
-/* "Fortuna.pyx":845
+/* "Fortuna.pyx":860
  *             w_pair[0] = cum_weight
  *         self.max_weight = optimized_data[-1][0]
  *         self.data = tuple(tuple(itm) for itm in optimized_data)             # <<<<<<<<<<<<<<
  * 
  * 
  */
 
@@ -21461,23 +22026,23 @@
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("genexpr", 0);
   __pyx_cur_scope = (struct __pyx_obj_7Fortuna___pyx_scope_struct_1_genexpr *)__pyx_tp_new_7Fortuna___pyx_scope_struct_1_genexpr(__pyx_ptype_7Fortuna___pyx_scope_struct_1_genexpr, __pyx_empty_tuple, NULL);
   if (unlikely(!__pyx_cur_scope)) {
     __pyx_cur_scope = ((struct __pyx_obj_7Fortuna___pyx_scope_struct_1_genexpr *)Py_None);
     __Pyx_INCREF(Py_None);
-    __PYX_ERR(0, 845, __pyx_L1_error)
+    __PYX_ERR(0, 860, __pyx_L1_error)
   } else {
     __Pyx_GOTREF((PyObject *)__pyx_cur_scope);
   }
   __pyx_cur_scope->__pyx_genexpr_arg_0 = __pyx_genexpr_arg_0;
   __Pyx_INCREF(__pyx_cur_scope->__pyx_genexpr_arg_0);
   __Pyx_GIVEREF(__pyx_cur_scope->__pyx_genexpr_arg_0);
   {
-    __pyx_CoroutineObject *gen = __Pyx_Generator_New((__pyx_coroutine_body_t) __pyx_gb_7Fortuna_22RelativeWeightedChoice_8__init___3generator, NULL, (PyObject *) __pyx_cur_scope, __pyx_n_s_genexpr, __pyx_n_s_RelativeWeightedChoice___init, __pyx_n_s_Fortuna); if (unlikely(!gen)) __PYX_ERR(0, 845, __pyx_L1_error)
+    __pyx_CoroutineObject *gen = __Pyx_Generator_New((__pyx_coroutine_body_t) __pyx_gb_7Fortuna_22RelativeWeightedChoice_8__init___3generator, NULL, (PyObject *) __pyx_cur_scope, __pyx_n_s_genexpr, __pyx_n_s_RelativeWeightedChoice___init, __pyx_n_s_Fortuna); if (unlikely(!gen)) __PYX_ERR(0, 860, __pyx_L1_error)
     __Pyx_DECREF(__pyx_cur_scope);
     __Pyx_RefNannyFinishContext();
     return (PyObject *) gen;
   }
 
   /* function exit code */
   __pyx_L1_error:;
@@ -21506,73 +22071,73 @@
     case 0: goto __pyx_L3_first_run;
     case 1: goto __pyx_L6_resume_from_yield;
     default: /* CPython raises the right error here */
     __Pyx_RefNannyFinishContext();
     return NULL;
   }
   __pyx_L3_first_run:;
-  if (unlikely(!__pyx_sent_value)) __PYX_ERR(0, 845, __pyx_L1_error)
-  if (unlikely(!__pyx_cur_scope->__pyx_genexpr_arg_0)) { __Pyx_RaiseUnboundLocalError(".0"); __PYX_ERR(0, 845, __pyx_L1_error) }
+  if (unlikely(!__pyx_sent_value)) __PYX_ERR(0, 860, __pyx_L1_error)
+  if (unlikely(!__pyx_cur_scope->__pyx_genexpr_arg_0)) { __Pyx_RaiseUnboundLocalError(".0"); __PYX_ERR(0, 860, __pyx_L1_error) }
   if (likely(PyList_CheckExact(__pyx_cur_scope->__pyx_genexpr_arg_0)) || PyTuple_CheckExact(__pyx_cur_scope->__pyx_genexpr_arg_0)) {
     __pyx_t_1 = __pyx_cur_scope->__pyx_genexpr_arg_0; __Pyx_INCREF(__pyx_t_1);
     __pyx_t_2 = 0;
     __pyx_t_3 = NULL;
   } else {
-    __pyx_t_2 = -1; __pyx_t_1 = PyObject_GetIter(__pyx_cur_scope->__pyx_genexpr_arg_0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 845, __pyx_L1_error)
+    __pyx_t_2 = -1; __pyx_t_1 = PyObject_GetIter(__pyx_cur_scope->__pyx_genexpr_arg_0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 860, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_3 = __Pyx_PyObject_GetIterNextFunc(__pyx_t_1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 845, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_GetIterNextFunc(__pyx_t_1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 860, __pyx_L1_error)
   }
   for (;;) {
     if (likely(!__pyx_t_3)) {
       if (likely(PyList_CheckExact(__pyx_t_1))) {
         {
           Py_ssize_t __pyx_temp = __Pyx_PyList_GET_SIZE(__pyx_t_1);
           #if !CYTHON_ASSUME_SAFE_MACROS
-          if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 845, __pyx_L1_error)
+          if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 860, __pyx_L1_error)
           #endif
           if (__pyx_t_2 >= __pyx_temp) break;
         }
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_4 = PyList_GET_ITEM(__pyx_t_1, __pyx_t_2); __Pyx_INCREF(__pyx_t_4); __pyx_t_2++; if (unlikely((0 < 0))) __PYX_ERR(0, 845, __pyx_L1_error)
+        __pyx_t_4 = PyList_GET_ITEM(__pyx_t_1, __pyx_t_2); __Pyx_INCREF(__pyx_t_4); __pyx_t_2++; if (unlikely((0 < 0))) __PYX_ERR(0, 860, __pyx_L1_error)
         #else
-        __pyx_t_4 = __Pyx_PySequence_ITEM(__pyx_t_1, __pyx_t_2); __pyx_t_2++; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 845, __pyx_L1_error)
+        __pyx_t_4 = __Pyx_PySequence_ITEM(__pyx_t_1, __pyx_t_2); __pyx_t_2++; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 860, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_4);
         #endif
       } else {
         {
           Py_ssize_t __pyx_temp = __Pyx_PyTuple_GET_SIZE(__pyx_t_1);
           #if !CYTHON_ASSUME_SAFE_MACROS
-          if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 845, __pyx_L1_error)
+          if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 860, __pyx_L1_error)
           #endif
           if (__pyx_t_2 >= __pyx_temp) break;
         }
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_4 = PyTuple_GET_ITEM(__pyx_t_1, __pyx_t_2); __Pyx_INCREF(__pyx_t_4); __pyx_t_2++; if (unlikely((0 < 0))) __PYX_ERR(0, 845, __pyx_L1_error)
+        __pyx_t_4 = PyTuple_GET_ITEM(__pyx_t_1, __pyx_t_2); __Pyx_INCREF(__pyx_t_4); __pyx_t_2++; if (unlikely((0 < 0))) __PYX_ERR(0, 860, __pyx_L1_error)
         #else
-        __pyx_t_4 = __Pyx_PySequence_ITEM(__pyx_t_1, __pyx_t_2); __pyx_t_2++; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 845, __pyx_L1_error)
+        __pyx_t_4 = __Pyx_PySequence_ITEM(__pyx_t_1, __pyx_t_2); __pyx_t_2++; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 860, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_4);
         #endif
       }
     } else {
       __pyx_t_4 = __pyx_t_3(__pyx_t_1);
       if (unlikely(!__pyx_t_4)) {
         PyObject* exc_type = PyErr_Occurred();
         if (exc_type) {
           if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-          else __PYX_ERR(0, 845, __pyx_L1_error)
+          else __PYX_ERR(0, 860, __pyx_L1_error)
         }
         break;
       }
       __Pyx_GOTREF(__pyx_t_4);
     }
     __Pyx_XGOTREF(__pyx_cur_scope->__pyx_v_itm);
     __Pyx_XDECREF_SET(__pyx_cur_scope->__pyx_v_itm, __pyx_t_4);
     __Pyx_GIVEREF(__pyx_t_4);
     __pyx_t_4 = 0;
-    __pyx_t_4 = __Pyx_PySequence_Tuple(__pyx_cur_scope->__pyx_v_itm); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 845, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PySequence_Tuple(__pyx_cur_scope->__pyx_v_itm); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 860, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __pyx_r = __pyx_t_4;
     __pyx_t_4 = 0;
     __Pyx_XGIVEREF(__pyx_t_1);
     __pyx_cur_scope->__pyx_t_0 = __pyx_t_1;
     __pyx_cur_scope->__pyx_t_1 = __pyx_t_2;
     __pyx_cur_scope->__pyx_t_2 = __pyx_t_3;
@@ -21584,15 +22149,15 @@
     return __pyx_r;
     __pyx_L6_resume_from_yield:;
     __pyx_t_1 = __pyx_cur_scope->__pyx_t_0;
     __pyx_cur_scope->__pyx_t_0 = 0;
     __Pyx_XGOTREF(__pyx_t_1);
     __pyx_t_2 = __pyx_cur_scope->__pyx_t_1;
     __pyx_t_3 = __pyx_cur_scope->__pyx_t_2;
-    if (unlikely(!__pyx_sent_value)) __PYX_ERR(0, 845, __pyx_L1_error)
+    if (unlikely(!__pyx_sent_value)) __PYX_ERR(0, 860, __pyx_L1_error)
   }
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   CYTHON_MAYBE_UNUSED_VAR(__pyx_cur_scope);
 
   /* function exit code */
   PyErr_SetNone(PyExc_StopIteration);
   goto __pyx_L0;
@@ -21608,15 +22173,15 @@
   #endif
   __pyx_generator->resume_label = -1;
   __Pyx_Coroutine_clear((PyObject*)__pyx_generator);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "Fortuna.pyx":826
+/* "Fortuna.pyx":841
  *     __slots__ = ("flat", "max_weight", "data")
  * 
  *     def __init__(self,             # <<<<<<<<<<<<<<
  *                  weighted_table: Iterable,
  *                  flat: bool = True):
  */
 
@@ -21634,288 +22199,288 @@
   PyObject *(*__pyx_t_4)(PyObject *);
   PyObject *__pyx_t_5 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__init__", 1);
 
-  /* "Fortuna.pyx":836
+  /* "Fortuna.pyx":851
  *         @return : Callable Instance
  *         """
  *         self.flat = flat             # <<<<<<<<<<<<<<
  *         optimized_data = sorted(
  *             [list(itm) for itm in weighted_table],
  */
-  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_flat, __pyx_v_flat) < 0) __PYX_ERR(0, 836, __pyx_L1_error)
+  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_flat, __pyx_v_flat) < 0) __PYX_ERR(0, 851, __pyx_L1_error)
 
-  /* "Fortuna.pyx":837
+  /* "Fortuna.pyx":852
  *         """
  *         self.flat = flat
  *         optimized_data = sorted(             # <<<<<<<<<<<<<<
  *             [list(itm) for itm in weighted_table],
  *             key=lambda x: x[0], reverse=True)
  */
   { /* enter inner scope */
 
-    /* "Fortuna.pyx":838
+    /* "Fortuna.pyx":853
  *         self.flat = flat
  *         optimized_data = sorted(
  *             [list(itm) for itm in weighted_table],             # <<<<<<<<<<<<<<
  *             key=lambda x: x[0], reverse=True)
  *         cum_weight = 0
  */
-    __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 838, __pyx_L5_error)
+    __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 853, __pyx_L5_error)
     __Pyx_GOTREF(__pyx_t_1);
     if (likely(PyList_CheckExact(__pyx_v_weighted_table)) || PyTuple_CheckExact(__pyx_v_weighted_table)) {
       __pyx_t_2 = __pyx_v_weighted_table; __Pyx_INCREF(__pyx_t_2);
       __pyx_t_3 = 0;
       __pyx_t_4 = NULL;
     } else {
-      __pyx_t_3 = -1; __pyx_t_2 = PyObject_GetIter(__pyx_v_weighted_table); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 838, __pyx_L5_error)
+      __pyx_t_3 = -1; __pyx_t_2 = PyObject_GetIter(__pyx_v_weighted_table); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 853, __pyx_L5_error)
       __Pyx_GOTREF(__pyx_t_2);
-      __pyx_t_4 = __Pyx_PyObject_GetIterNextFunc(__pyx_t_2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 838, __pyx_L5_error)
+      __pyx_t_4 = __Pyx_PyObject_GetIterNextFunc(__pyx_t_2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 853, __pyx_L5_error)
     }
     for (;;) {
       if (likely(!__pyx_t_4)) {
         if (likely(PyList_CheckExact(__pyx_t_2))) {
           {
             Py_ssize_t __pyx_temp = __Pyx_PyList_GET_SIZE(__pyx_t_2);
             #if !CYTHON_ASSUME_SAFE_MACROS
-            if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 838, __pyx_L5_error)
+            if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 853, __pyx_L5_error)
             #endif
             if (__pyx_t_3 >= __pyx_temp) break;
           }
           #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-          __pyx_t_5 = PyList_GET_ITEM(__pyx_t_2, __pyx_t_3); __Pyx_INCREF(__pyx_t_5); __pyx_t_3++; if (unlikely((0 < 0))) __PYX_ERR(0, 838, __pyx_L5_error)
+          __pyx_t_5 = PyList_GET_ITEM(__pyx_t_2, __pyx_t_3); __Pyx_INCREF(__pyx_t_5); __pyx_t_3++; if (unlikely((0 < 0))) __PYX_ERR(0, 853, __pyx_L5_error)
           #else
-          __pyx_t_5 = __Pyx_PySequence_ITEM(__pyx_t_2, __pyx_t_3); __pyx_t_3++; if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 838, __pyx_L5_error)
+          __pyx_t_5 = __Pyx_PySequence_ITEM(__pyx_t_2, __pyx_t_3); __pyx_t_3++; if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 853, __pyx_L5_error)
           __Pyx_GOTREF(__pyx_t_5);
           #endif
         } else {
           {
             Py_ssize_t __pyx_temp = __Pyx_PyTuple_GET_SIZE(__pyx_t_2);
             #if !CYTHON_ASSUME_SAFE_MACROS
-            if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 838, __pyx_L5_error)
+            if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 853, __pyx_L5_error)
             #endif
             if (__pyx_t_3 >= __pyx_temp) break;
           }
           #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-          __pyx_t_5 = PyTuple_GET_ITEM(__pyx_t_2, __pyx_t_3); __Pyx_INCREF(__pyx_t_5); __pyx_t_3++; if (unlikely((0 < 0))) __PYX_ERR(0, 838, __pyx_L5_error)
+          __pyx_t_5 = PyTuple_GET_ITEM(__pyx_t_2, __pyx_t_3); __Pyx_INCREF(__pyx_t_5); __pyx_t_3++; if (unlikely((0 < 0))) __PYX_ERR(0, 853, __pyx_L5_error)
           #else
-          __pyx_t_5 = __Pyx_PySequence_ITEM(__pyx_t_2, __pyx_t_3); __pyx_t_3++; if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 838, __pyx_L5_error)
+          __pyx_t_5 = __Pyx_PySequence_ITEM(__pyx_t_2, __pyx_t_3); __pyx_t_3++; if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 853, __pyx_L5_error)
           __Pyx_GOTREF(__pyx_t_5);
           #endif
         }
       } else {
         __pyx_t_5 = __pyx_t_4(__pyx_t_2);
         if (unlikely(!__pyx_t_5)) {
           PyObject* exc_type = PyErr_Occurred();
           if (exc_type) {
             if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-            else __PYX_ERR(0, 838, __pyx_L5_error)
+            else __PYX_ERR(0, 853, __pyx_L5_error)
           }
           break;
         }
         __Pyx_GOTREF(__pyx_t_5);
       }
       __Pyx_XDECREF_SET(__pyx_8genexpr1__pyx_v_itm, __pyx_t_5);
       __pyx_t_5 = 0;
-      __pyx_t_5 = PySequence_List(__pyx_8genexpr1__pyx_v_itm); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 838, __pyx_L5_error)
+      __pyx_t_5 = PySequence_List(__pyx_8genexpr1__pyx_v_itm); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 853, __pyx_L5_error)
       __Pyx_GOTREF(__pyx_t_5);
-      if (unlikely(__Pyx_ListComp_Append(__pyx_t_1, (PyObject*)__pyx_t_5))) __PYX_ERR(0, 838, __pyx_L5_error)
+      if (unlikely(__Pyx_ListComp_Append(__pyx_t_1, (PyObject*)__pyx_t_5))) __PYX_ERR(0, 853, __pyx_L5_error)
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     }
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_8genexpr1__pyx_v_itm); __pyx_8genexpr1__pyx_v_itm = 0;
     goto __pyx_L9_exit_scope;
     __pyx_L5_error:;
     __Pyx_XDECREF(__pyx_8genexpr1__pyx_v_itm); __pyx_8genexpr1__pyx_v_itm = 0;
     goto __pyx_L1_error;
     __pyx_L9_exit_scope:;
   } /* exit inner scope */
 
-  /* "Fortuna.pyx":837
+  /* "Fortuna.pyx":852
  *         """
  *         self.flat = flat
  *         optimized_data = sorted(             # <<<<<<<<<<<<<<
  *             [list(itm) for itm in weighted_table],
  *             key=lambda x: x[0], reverse=True)
  */
-  __pyx_t_2 = PyTuple_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 837, __pyx_L1_error)
+  __pyx_t_2 = PyTuple_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 852, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_GIVEREF(__pyx_t_1);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_t_1)) __PYX_ERR(0, 837, __pyx_L1_error);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_t_1)) __PYX_ERR(0, 852, __pyx_L1_error);
   __pyx_t_1 = 0;
 
-  /* "Fortuna.pyx":839
+  /* "Fortuna.pyx":854
  *         optimized_data = sorted(
  *             [list(itm) for itm in weighted_table],
  *             key=lambda x: x[0], reverse=True)             # <<<<<<<<<<<<<<
  *         cum_weight = 0
  *         for w_pair in optimized_data:
  */
-  __pyx_t_1 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 839, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 854, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_7Fortuna_22RelativeWeightedChoice_8__init___lambda, 0, __pyx_n_s_RelativeWeightedChoice___init_2, NULL, __pyx_n_s_Fortuna, __pyx_d, NULL); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 839, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_7Fortuna_22RelativeWeightedChoice_8__init___lambda, 0, __pyx_n_s_RelativeWeightedChoice___init_2, NULL, __pyx_n_s_Fortuna, __pyx_d, NULL); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 854, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_key, __pyx_t_5) < 0) __PYX_ERR(0, 839, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_key, __pyx_t_5) < 0) __PYX_ERR(0, 854, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_reverse, Py_True) < 0) __PYX_ERR(0, 839, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_reverse, Py_True) < 0) __PYX_ERR(0, 854, __pyx_L1_error)
 
-  /* "Fortuna.pyx":837
+  /* "Fortuna.pyx":852
  *         """
  *         self.flat = flat
  *         optimized_data = sorted(             # <<<<<<<<<<<<<<
  *             [list(itm) for itm in weighted_table],
  *             key=lambda x: x[0], reverse=True)
  */
-  __pyx_t_5 = __Pyx_PyObject_Call(__pyx_builtin_sorted, __pyx_t_2, __pyx_t_1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 837, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_Call(__pyx_builtin_sorted, __pyx_t_2, __pyx_t_1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 852, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_v_optimized_data = __pyx_t_5;
   __pyx_t_5 = 0;
 
-  /* "Fortuna.pyx":840
+  /* "Fortuna.pyx":855
  *             [list(itm) for itm in weighted_table],
  *             key=lambda x: x[0], reverse=True)
  *         cum_weight = 0             # <<<<<<<<<<<<<<
  *         for w_pair in optimized_data:
  *             cum_weight += w_pair[0]
  */
   __Pyx_INCREF(__pyx_int_0);
   __pyx_v_cum_weight = __pyx_int_0;
 
-  /* "Fortuna.pyx":841
+  /* "Fortuna.pyx":856
  *             key=lambda x: x[0], reverse=True)
  *         cum_weight = 0
  *         for w_pair in optimized_data:             # <<<<<<<<<<<<<<
  *             cum_weight += w_pair[0]
  *             w_pair[0] = cum_weight
  */
   if (likely(PyList_CheckExact(__pyx_v_optimized_data)) || PyTuple_CheckExact(__pyx_v_optimized_data)) {
     __pyx_t_5 = __pyx_v_optimized_data; __Pyx_INCREF(__pyx_t_5);
     __pyx_t_3 = 0;
     __pyx_t_4 = NULL;
   } else {
-    __pyx_t_3 = -1; __pyx_t_5 = PyObject_GetIter(__pyx_v_optimized_data); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 841, __pyx_L1_error)
+    __pyx_t_3 = -1; __pyx_t_5 = PyObject_GetIter(__pyx_v_optimized_data); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 856, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
-    __pyx_t_4 = __Pyx_PyObject_GetIterNextFunc(__pyx_t_5); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 841, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_GetIterNextFunc(__pyx_t_5); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 856, __pyx_L1_error)
   }
   for (;;) {
     if (likely(!__pyx_t_4)) {
       if (likely(PyList_CheckExact(__pyx_t_5))) {
         {
           Py_ssize_t __pyx_temp = __Pyx_PyList_GET_SIZE(__pyx_t_5);
           #if !CYTHON_ASSUME_SAFE_MACROS
-          if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 841, __pyx_L1_error)
+          if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 856, __pyx_L1_error)
           #endif
           if (__pyx_t_3 >= __pyx_temp) break;
         }
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_1 = PyList_GET_ITEM(__pyx_t_5, __pyx_t_3); __Pyx_INCREF(__pyx_t_1); __pyx_t_3++; if (unlikely((0 < 0))) __PYX_ERR(0, 841, __pyx_L1_error)
+        __pyx_t_1 = PyList_GET_ITEM(__pyx_t_5, __pyx_t_3); __Pyx_INCREF(__pyx_t_1); __pyx_t_3++; if (unlikely((0 < 0))) __PYX_ERR(0, 856, __pyx_L1_error)
         #else
-        __pyx_t_1 = __Pyx_PySequence_ITEM(__pyx_t_5, __pyx_t_3); __pyx_t_3++; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 841, __pyx_L1_error)
+        __pyx_t_1 = __Pyx_PySequence_ITEM(__pyx_t_5, __pyx_t_3); __pyx_t_3++; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 856, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_1);
         #endif
       } else {
         {
           Py_ssize_t __pyx_temp = __Pyx_PyTuple_GET_SIZE(__pyx_t_5);
           #if !CYTHON_ASSUME_SAFE_MACROS
-          if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 841, __pyx_L1_error)
+          if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 856, __pyx_L1_error)
           #endif
           if (__pyx_t_3 >= __pyx_temp) break;
         }
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_1 = PyTuple_GET_ITEM(__pyx_t_5, __pyx_t_3); __Pyx_INCREF(__pyx_t_1); __pyx_t_3++; if (unlikely((0 < 0))) __PYX_ERR(0, 841, __pyx_L1_error)
+        __pyx_t_1 = PyTuple_GET_ITEM(__pyx_t_5, __pyx_t_3); __Pyx_INCREF(__pyx_t_1); __pyx_t_3++; if (unlikely((0 < 0))) __PYX_ERR(0, 856, __pyx_L1_error)
         #else
-        __pyx_t_1 = __Pyx_PySequence_ITEM(__pyx_t_5, __pyx_t_3); __pyx_t_3++; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 841, __pyx_L1_error)
+        __pyx_t_1 = __Pyx_PySequence_ITEM(__pyx_t_5, __pyx_t_3); __pyx_t_3++; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 856, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_1);
         #endif
       }
     } else {
       __pyx_t_1 = __pyx_t_4(__pyx_t_5);
       if (unlikely(!__pyx_t_1)) {
         PyObject* exc_type = PyErr_Occurred();
         if (exc_type) {
           if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-          else __PYX_ERR(0, 841, __pyx_L1_error)
+          else __PYX_ERR(0, 856, __pyx_L1_error)
         }
         break;
       }
       __Pyx_GOTREF(__pyx_t_1);
     }
     __Pyx_XDECREF_SET(__pyx_v_w_pair, __pyx_t_1);
     __pyx_t_1 = 0;
 
-    /* "Fortuna.pyx":842
+    /* "Fortuna.pyx":857
  *         cum_weight = 0
  *         for w_pair in optimized_data:
  *             cum_weight += w_pair[0]             # <<<<<<<<<<<<<<
  *             w_pair[0] = cum_weight
  *         self.max_weight = optimized_data[-1][0]
  */
-    __pyx_t_1 = __Pyx_GetItemInt(__pyx_v_w_pair, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 842, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_GetItemInt(__pyx_v_w_pair, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 857, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_2 = PyNumber_InPlaceAdd(__pyx_v_cum_weight, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 842, __pyx_L1_error)
+    __pyx_t_2 = PyNumber_InPlaceAdd(__pyx_v_cum_weight, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 857, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_DECREF_SET(__pyx_v_cum_weight, __pyx_t_2);
     __pyx_t_2 = 0;
 
-    /* "Fortuna.pyx":843
+    /* "Fortuna.pyx":858
  *         for w_pair in optimized_data:
  *             cum_weight += w_pair[0]
  *             w_pair[0] = cum_weight             # <<<<<<<<<<<<<<
  *         self.max_weight = optimized_data[-1][0]
  *         self.data = tuple(tuple(itm) for itm in optimized_data)
  */
-    if (unlikely((__Pyx_SetItemInt(__pyx_v_w_pair, 0, __pyx_v_cum_weight, long, 1, __Pyx_PyInt_From_long, 0, 0, 1) < 0))) __PYX_ERR(0, 843, __pyx_L1_error)
+    if (unlikely((__Pyx_SetItemInt(__pyx_v_w_pair, 0, __pyx_v_cum_weight, long, 1, __Pyx_PyInt_From_long, 0, 0, 1) < 0))) __PYX_ERR(0, 858, __pyx_L1_error)
 
-    /* "Fortuna.pyx":841
+    /* "Fortuna.pyx":856
  *             key=lambda x: x[0], reverse=True)
  *         cum_weight = 0
  *         for w_pair in optimized_data:             # <<<<<<<<<<<<<<
  *             cum_weight += w_pair[0]
  *             w_pair[0] = cum_weight
  */
   }
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
-  /* "Fortuna.pyx":844
+  /* "Fortuna.pyx":859
  *             cum_weight += w_pair[0]
  *             w_pair[0] = cum_weight
  *         self.max_weight = optimized_data[-1][0]             # <<<<<<<<<<<<<<
  *         self.data = tuple(tuple(itm) for itm in optimized_data)
  * 
  */
-  __pyx_t_5 = __Pyx_GetItemInt(__pyx_v_optimized_data, -1L, long, 1, __Pyx_PyInt_From_long, 0, 1, 1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 844, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_GetItemInt(__pyx_v_optimized_data, -1L, long, 1, __Pyx_PyInt_From_long, 0, 1, 1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 859, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_2 = __Pyx_GetItemInt(__pyx_t_5, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 844, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_GetItemInt(__pyx_t_5, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 859, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_max_weight, __pyx_t_2) < 0) __PYX_ERR(0, 844, __pyx_L1_error)
+  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_max_weight, __pyx_t_2) < 0) __PYX_ERR(0, 859, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "Fortuna.pyx":845
+  /* "Fortuna.pyx":860
  *             w_pair[0] = cum_weight
  *         self.max_weight = optimized_data[-1][0]
  *         self.data = tuple(tuple(itm) for itm in optimized_data)             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_t_2 = __pyx_pf_7Fortuna_22RelativeWeightedChoice_8__init___1genexpr(NULL, __pyx_v_optimized_data); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 845, __pyx_L1_error)
+  __pyx_t_2 = __pyx_pf_7Fortuna_22RelativeWeightedChoice_8__init___1genexpr(NULL, __pyx_v_optimized_data); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 860, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_5 = __Pyx_PySequence_Tuple(__pyx_t_2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 845, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PySequence_Tuple(__pyx_t_2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 860, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_data, __pyx_t_5) < 0) __PYX_ERR(0, 845, __pyx_L1_error)
+  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_data, __pyx_t_5) < 0) __PYX_ERR(0, 860, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
-  /* "Fortuna.pyx":826
+  /* "Fortuna.pyx":841
  *     __slots__ = ("flat", "max_weight", "data")
  * 
  *     def __init__(self,             # <<<<<<<<<<<<<<
  *                  weighted_table: Iterable,
  *                  flat: bool = True):
  */
 
@@ -21935,15 +22500,15 @@
   __Pyx_XDECREF(__pyx_8genexpr1__pyx_v_itm);
   __Pyx_XDECREF(__pyx_gb_7Fortuna_22RelativeWeightedChoice_8__init___3generator);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "Fortuna.pyx":852
+/* "Fortuna.pyx":867
  *     __slots__ = ("flat", "max_weight", "data")
  * 
  *     def __init__(self,             # <<<<<<<<<<<<<<
  *                  weighted_table: Iterable,
  *                  flat: bool = True):
  */
 
@@ -21985,15 +22550,15 @@
   __pyx_nargs = PyTuple_Size(__pyx_args); if (unlikely(__pyx_nargs < 0)) return NULL;
   #endif
   #endif
   __pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
   {
     PyObject **__pyx_pyargnames[] = {&__pyx_n_s_self,&__pyx_n_s_weighted_table,&__pyx_n_s_flat,0};
 
-    /* "Fortuna.pyx":854
+    /* "Fortuna.pyx":869
  *     def __init__(self,
  *                  weighted_table: Iterable,
  *                  flat: bool = True):             # <<<<<<<<<<<<<<
  *         """
  *         @param weighted_table : Table of weighted pairs.
  */
     values[2] = __Pyx_Arg_NewRef_FASTCALL(((PyObject *)((PyObject *)Py_True)));
@@ -22012,37 +22577,37 @@
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_self)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 852, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 867, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_weighted_table)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[1]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 852, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 867, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("__init__", 0, 2, 3, 1); __PYX_ERR(0, 852, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__init__", 0, 2, 3, 1); __PYX_ERR(0, 867, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (kw_args > 0) {
           PyObject* value = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_flat);
           if (value) { values[2] = __Pyx_Arg_NewRef_FASTCALL(value); kw_args--; }
-          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 852, __pyx_L3_error)
+          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 867, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "__init__") < 0)) __PYX_ERR(0, 852, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "__init__") < 0)) __PYX_ERR(0, 867, __pyx_L3_error)
       }
     } else {
       switch (__pyx_nargs) {
         case  3: values[2] = __Pyx_Arg_FASTCALL(__pyx_args, 2);
         CYTHON_FALLTHROUGH;
         case  2: values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
         values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
@@ -22052,15 +22617,15 @@
     }
     __pyx_v_self = values[0];
     __pyx_v_weighted_table = values[1];
     __pyx_v_flat = values[2];
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__init__", 0, 2, 3, __pyx_nargs); __PYX_ERR(0, 852, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__init__", 0, 2, 3, __pyx_nargs); __PYX_ERR(0, 867, __pyx_L3_error)
   __pyx_L6_skip:;
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
@@ -22068,15 +22633,15 @@
   }
   __Pyx_AddTraceback("Fortuna.CumulativeWeightedChoice.__init__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_7Fortuna_24CumulativeWeightedChoice___init__(__pyx_self, __pyx_v_self, __pyx_v_weighted_table, __pyx_v_flat);
 
-  /* "Fortuna.pyx":852
+  /* "Fortuna.pyx":867
  *     __slots__ = ("flat", "max_weight", "data")
  * 
  *     def __init__(self,             # <<<<<<<<<<<<<<
  *                  weighted_table: Iterable,
  *                  flat: bool = True):
  */
 
@@ -22087,15 +22652,15 @@
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "Fortuna.pyx":864
+/* "Fortuna.pyx":879
  *         """
  *         self.flat = flat
  *         data = sorted([list(itm) for itm in weighted_table], key=lambda x: x[0])             # <<<<<<<<<<<<<<
  *         prev_weight = 0
  *         for w_pair in data:
  */
 
@@ -22148,31 +22713,31 @@
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_x)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 864, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 879, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "lambda2") < 0)) __PYX_ERR(0, 864, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "lambda2") < 0)) __PYX_ERR(0, 879, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs != 1)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
     }
     __pyx_v_x = values[0];
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("lambda2", 1, 1, 1, __pyx_nargs); __PYX_ERR(0, 864, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("lambda2", 1, 1, 1, __pyx_nargs); __PYX_ERR(0, 879, __pyx_L3_error)
   __pyx_L6_skip:;
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
@@ -22200,15 +22765,15 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("lambda2", 1);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_GetItemInt(__pyx_v_x, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 864, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_GetItemInt(__pyx_v_x, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 879, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -22217,15 +22782,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "Fortuna.pyx":868
+/* "Fortuna.pyx":883
  *         for w_pair in data:
  *             w_pair[0], prev_weight = w_pair[0] - prev_weight, w_pair[0]
  *         optimized_data = sorted(data, key=lambda x: x[0], reverse=True)             # <<<<<<<<<<<<<<
  *         cum_weight = 0
  *         for w_pair in optimized_data:
  */
 
@@ -22278,31 +22843,31 @@
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_x)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 868, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 883, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "lambda3") < 0)) __PYX_ERR(0, 868, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "lambda3") < 0)) __PYX_ERR(0, 883, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs != 1)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
     }
     __pyx_v_x = values[0];
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("lambda3", 1, 1, 1, __pyx_nargs); __PYX_ERR(0, 868, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("lambda3", 1, 1, 1, __pyx_nargs); __PYX_ERR(0, 883, __pyx_L3_error)
   __pyx_L6_skip:;
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
@@ -22330,15 +22895,15 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("lambda3", 1);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_GetItemInt(__pyx_v_x, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 868, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_GetItemInt(__pyx_v_x, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 883, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -22348,15 +22913,15 @@
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 static PyObject *__pyx_gb_7Fortuna_24CumulativeWeightedChoice_8__init___4generator1(__pyx_CoroutineObject *__pyx_generator, CYTHON_UNUSED PyThreadState *__pyx_tstate, PyObject *__pyx_sent_value); /* proto */
 
-/* "Fortuna.pyx":874
+/* "Fortuna.pyx":889
  *             w_pair[0] = cum_weight
  *         self.max_weight = optimized_data[-1][0]
  *         self.data = tuple(tuple(itm) for itm in optimized_data)             # <<<<<<<<<<<<<<
  * 
  * 
  */
 
@@ -22368,23 +22933,23 @@
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("genexpr", 0);
   __pyx_cur_scope = (struct __pyx_obj_7Fortuna___pyx_scope_struct_2_genexpr *)__pyx_tp_new_7Fortuna___pyx_scope_struct_2_genexpr(__pyx_ptype_7Fortuna___pyx_scope_struct_2_genexpr, __pyx_empty_tuple, NULL);
   if (unlikely(!__pyx_cur_scope)) {
     __pyx_cur_scope = ((struct __pyx_obj_7Fortuna___pyx_scope_struct_2_genexpr *)Py_None);
     __Pyx_INCREF(Py_None);
-    __PYX_ERR(0, 874, __pyx_L1_error)
+    __PYX_ERR(0, 889, __pyx_L1_error)
   } else {
     __Pyx_GOTREF((PyObject *)__pyx_cur_scope);
   }
   __pyx_cur_scope->__pyx_genexpr_arg_0 = __pyx_genexpr_arg_0;
   __Pyx_INCREF(__pyx_cur_scope->__pyx_genexpr_arg_0);
   __Pyx_GIVEREF(__pyx_cur_scope->__pyx_genexpr_arg_0);
   {
-    __pyx_CoroutineObject *gen = __Pyx_Generator_New((__pyx_coroutine_body_t) __pyx_gb_7Fortuna_24CumulativeWeightedChoice_8__init___4generator1, NULL, (PyObject *) __pyx_cur_scope, __pyx_n_s_genexpr, __pyx_n_s_CumulativeWeightedChoice___init, __pyx_n_s_Fortuna); if (unlikely(!gen)) __PYX_ERR(0, 874, __pyx_L1_error)
+    __pyx_CoroutineObject *gen = __Pyx_Generator_New((__pyx_coroutine_body_t) __pyx_gb_7Fortuna_24CumulativeWeightedChoice_8__init___4generator1, NULL, (PyObject *) __pyx_cur_scope, __pyx_n_s_genexpr, __pyx_n_s_CumulativeWeightedChoice___init, __pyx_n_s_Fortuna); if (unlikely(!gen)) __PYX_ERR(0, 889, __pyx_L1_error)
     __Pyx_DECREF(__pyx_cur_scope);
     __Pyx_RefNannyFinishContext();
     return (PyObject *) gen;
   }
 
   /* function exit code */
   __pyx_L1_error:;
@@ -22413,73 +22978,73 @@
     case 0: goto __pyx_L3_first_run;
     case 1: goto __pyx_L6_resume_from_yield;
     default: /* CPython raises the right error here */
     __Pyx_RefNannyFinishContext();
     return NULL;
   }
   __pyx_L3_first_run:;
-  if (unlikely(!__pyx_sent_value)) __PYX_ERR(0, 874, __pyx_L1_error)
-  if (unlikely(!__pyx_cur_scope->__pyx_genexpr_arg_0)) { __Pyx_RaiseUnboundLocalError(".0"); __PYX_ERR(0, 874, __pyx_L1_error) }
+  if (unlikely(!__pyx_sent_value)) __PYX_ERR(0, 889, __pyx_L1_error)
+  if (unlikely(!__pyx_cur_scope->__pyx_genexpr_arg_0)) { __Pyx_RaiseUnboundLocalError(".0"); __PYX_ERR(0, 889, __pyx_L1_error) }
   if (likely(PyList_CheckExact(__pyx_cur_scope->__pyx_genexpr_arg_0)) || PyTuple_CheckExact(__pyx_cur_scope->__pyx_genexpr_arg_0)) {
     __pyx_t_1 = __pyx_cur_scope->__pyx_genexpr_arg_0; __Pyx_INCREF(__pyx_t_1);
     __pyx_t_2 = 0;
     __pyx_t_3 = NULL;
   } else {
-    __pyx_t_2 = -1; __pyx_t_1 = PyObject_GetIter(__pyx_cur_scope->__pyx_genexpr_arg_0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 874, __pyx_L1_error)
+    __pyx_t_2 = -1; __pyx_t_1 = PyObject_GetIter(__pyx_cur_scope->__pyx_genexpr_arg_0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 889, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_3 = __Pyx_PyObject_GetIterNextFunc(__pyx_t_1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 874, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_GetIterNextFunc(__pyx_t_1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 889, __pyx_L1_error)
   }
   for (;;) {
     if (likely(!__pyx_t_3)) {
       if (likely(PyList_CheckExact(__pyx_t_1))) {
         {
           Py_ssize_t __pyx_temp = __Pyx_PyList_GET_SIZE(__pyx_t_1);
           #if !CYTHON_ASSUME_SAFE_MACROS
-          if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 874, __pyx_L1_error)
+          if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 889, __pyx_L1_error)
           #endif
           if (__pyx_t_2 >= __pyx_temp) break;
         }
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_4 = PyList_GET_ITEM(__pyx_t_1, __pyx_t_2); __Pyx_INCREF(__pyx_t_4); __pyx_t_2++; if (unlikely((0 < 0))) __PYX_ERR(0, 874, __pyx_L1_error)
+        __pyx_t_4 = PyList_GET_ITEM(__pyx_t_1, __pyx_t_2); __Pyx_INCREF(__pyx_t_4); __pyx_t_2++; if (unlikely((0 < 0))) __PYX_ERR(0, 889, __pyx_L1_error)
         #else
-        __pyx_t_4 = __Pyx_PySequence_ITEM(__pyx_t_1, __pyx_t_2); __pyx_t_2++; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 874, __pyx_L1_error)
+        __pyx_t_4 = __Pyx_PySequence_ITEM(__pyx_t_1, __pyx_t_2); __pyx_t_2++; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 889, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_4);
         #endif
       } else {
         {
           Py_ssize_t __pyx_temp = __Pyx_PyTuple_GET_SIZE(__pyx_t_1);
           #if !CYTHON_ASSUME_SAFE_MACROS
-          if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 874, __pyx_L1_error)
+          if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 889, __pyx_L1_error)
           #endif
           if (__pyx_t_2 >= __pyx_temp) break;
         }
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_4 = PyTuple_GET_ITEM(__pyx_t_1, __pyx_t_2); __Pyx_INCREF(__pyx_t_4); __pyx_t_2++; if (unlikely((0 < 0))) __PYX_ERR(0, 874, __pyx_L1_error)
+        __pyx_t_4 = PyTuple_GET_ITEM(__pyx_t_1, __pyx_t_2); __Pyx_INCREF(__pyx_t_4); __pyx_t_2++; if (unlikely((0 < 0))) __PYX_ERR(0, 889, __pyx_L1_error)
         #else
-        __pyx_t_4 = __Pyx_PySequence_ITEM(__pyx_t_1, __pyx_t_2); __pyx_t_2++; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 874, __pyx_L1_error)
+        __pyx_t_4 = __Pyx_PySequence_ITEM(__pyx_t_1, __pyx_t_2); __pyx_t_2++; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 889, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_4);
         #endif
       }
     } else {
       __pyx_t_4 = __pyx_t_3(__pyx_t_1);
       if (unlikely(!__pyx_t_4)) {
         PyObject* exc_type = PyErr_Occurred();
         if (exc_type) {
           if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-          else __PYX_ERR(0, 874, __pyx_L1_error)
+          else __PYX_ERR(0, 889, __pyx_L1_error)
         }
         break;
       }
       __Pyx_GOTREF(__pyx_t_4);
     }
     __Pyx_XGOTREF(__pyx_cur_scope->__pyx_v_itm);
     __Pyx_XDECREF_SET(__pyx_cur_scope->__pyx_v_itm, __pyx_t_4);
     __Pyx_GIVEREF(__pyx_t_4);
     __pyx_t_4 = 0;
-    __pyx_t_4 = __Pyx_PySequence_Tuple(__pyx_cur_scope->__pyx_v_itm); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 874, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PySequence_Tuple(__pyx_cur_scope->__pyx_v_itm); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 889, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __pyx_r = __pyx_t_4;
     __pyx_t_4 = 0;
     __Pyx_XGIVEREF(__pyx_t_1);
     __pyx_cur_scope->__pyx_t_0 = __pyx_t_1;
     __pyx_cur_scope->__pyx_t_1 = __pyx_t_2;
     __pyx_cur_scope->__pyx_t_2 = __pyx_t_3;
@@ -22491,15 +23056,15 @@
     return __pyx_r;
     __pyx_L6_resume_from_yield:;
     __pyx_t_1 = __pyx_cur_scope->__pyx_t_0;
     __pyx_cur_scope->__pyx_t_0 = 0;
     __Pyx_XGOTREF(__pyx_t_1);
     __pyx_t_2 = __pyx_cur_scope->__pyx_t_1;
     __pyx_t_3 = __pyx_cur_scope->__pyx_t_2;
-    if (unlikely(!__pyx_sent_value)) __PYX_ERR(0, 874, __pyx_L1_error)
+    if (unlikely(!__pyx_sent_value)) __PYX_ERR(0, 889, __pyx_L1_error)
   }
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   CYTHON_MAYBE_UNUSED_VAR(__pyx_cur_scope);
 
   /* function exit code */
   PyErr_SetNone(PyExc_StopIteration);
   goto __pyx_L0;
@@ -22515,15 +23080,15 @@
   #endif
   __pyx_generator->resume_label = -1;
   __Pyx_Coroutine_clear((PyObject*)__pyx_generator);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "Fortuna.pyx":852
+/* "Fortuna.pyx":867
  *     __slots__ = ("flat", "max_weight", "data")
  * 
  *     def __init__(self,             # <<<<<<<<<<<<<<
  *                  weighted_table: Iterable,
  *                  flat: bool = True):
  */
 
@@ -22543,382 +23108,382 @@
   PyObject *(*__pyx_t_4)(PyObject *);
   PyObject *__pyx_t_5 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__init__", 1);
 
-  /* "Fortuna.pyx":863
+  /* "Fortuna.pyx":878
  *         Note: Logic dictates Cumulative Weights must be unique!
  *         """
  *         self.flat = flat             # <<<<<<<<<<<<<<
  *         data = sorted([list(itm) for itm in weighted_table], key=lambda x: x[0])
  *         prev_weight = 0
  */
-  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_flat, __pyx_v_flat) < 0) __PYX_ERR(0, 863, __pyx_L1_error)
+  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_flat, __pyx_v_flat) < 0) __PYX_ERR(0, 878, __pyx_L1_error)
 
-  /* "Fortuna.pyx":864
+  /* "Fortuna.pyx":879
  *         """
  *         self.flat = flat
  *         data = sorted([list(itm) for itm in weighted_table], key=lambda x: x[0])             # <<<<<<<<<<<<<<
  *         prev_weight = 0
  *         for w_pair in data:
  */
   { /* enter inner scope */
-    __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 864, __pyx_L5_error)
+    __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 879, __pyx_L5_error)
     __Pyx_GOTREF(__pyx_t_1);
     if (likely(PyList_CheckExact(__pyx_v_weighted_table)) || PyTuple_CheckExact(__pyx_v_weighted_table)) {
       __pyx_t_2 = __pyx_v_weighted_table; __Pyx_INCREF(__pyx_t_2);
       __pyx_t_3 = 0;
       __pyx_t_4 = NULL;
     } else {
-      __pyx_t_3 = -1; __pyx_t_2 = PyObject_GetIter(__pyx_v_weighted_table); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 864, __pyx_L5_error)
+      __pyx_t_3 = -1; __pyx_t_2 = PyObject_GetIter(__pyx_v_weighted_table); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 879, __pyx_L5_error)
       __Pyx_GOTREF(__pyx_t_2);
-      __pyx_t_4 = __Pyx_PyObject_GetIterNextFunc(__pyx_t_2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 864, __pyx_L5_error)
+      __pyx_t_4 = __Pyx_PyObject_GetIterNextFunc(__pyx_t_2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 879, __pyx_L5_error)
     }
     for (;;) {
       if (likely(!__pyx_t_4)) {
         if (likely(PyList_CheckExact(__pyx_t_2))) {
           {
             Py_ssize_t __pyx_temp = __Pyx_PyList_GET_SIZE(__pyx_t_2);
             #if !CYTHON_ASSUME_SAFE_MACROS
-            if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 864, __pyx_L5_error)
+            if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 879, __pyx_L5_error)
             #endif
             if (__pyx_t_3 >= __pyx_temp) break;
           }
           #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-          __pyx_t_5 = PyList_GET_ITEM(__pyx_t_2, __pyx_t_3); __Pyx_INCREF(__pyx_t_5); __pyx_t_3++; if (unlikely((0 < 0))) __PYX_ERR(0, 864, __pyx_L5_error)
+          __pyx_t_5 = PyList_GET_ITEM(__pyx_t_2, __pyx_t_3); __Pyx_INCREF(__pyx_t_5); __pyx_t_3++; if (unlikely((0 < 0))) __PYX_ERR(0, 879, __pyx_L5_error)
           #else
-          __pyx_t_5 = __Pyx_PySequence_ITEM(__pyx_t_2, __pyx_t_3); __pyx_t_3++; if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 864, __pyx_L5_error)
+          __pyx_t_5 = __Pyx_PySequence_ITEM(__pyx_t_2, __pyx_t_3); __pyx_t_3++; if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 879, __pyx_L5_error)
           __Pyx_GOTREF(__pyx_t_5);
           #endif
         } else {
           {
             Py_ssize_t __pyx_temp = __Pyx_PyTuple_GET_SIZE(__pyx_t_2);
             #if !CYTHON_ASSUME_SAFE_MACROS
-            if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 864, __pyx_L5_error)
+            if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 879, __pyx_L5_error)
             #endif
             if (__pyx_t_3 >= __pyx_temp) break;
           }
           #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-          __pyx_t_5 = PyTuple_GET_ITEM(__pyx_t_2, __pyx_t_3); __Pyx_INCREF(__pyx_t_5); __pyx_t_3++; if (unlikely((0 < 0))) __PYX_ERR(0, 864, __pyx_L5_error)
+          __pyx_t_5 = PyTuple_GET_ITEM(__pyx_t_2, __pyx_t_3); __Pyx_INCREF(__pyx_t_5); __pyx_t_3++; if (unlikely((0 < 0))) __PYX_ERR(0, 879, __pyx_L5_error)
           #else
-          __pyx_t_5 = __Pyx_PySequence_ITEM(__pyx_t_2, __pyx_t_3); __pyx_t_3++; if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 864, __pyx_L5_error)
+          __pyx_t_5 = __Pyx_PySequence_ITEM(__pyx_t_2, __pyx_t_3); __pyx_t_3++; if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 879, __pyx_L5_error)
           __Pyx_GOTREF(__pyx_t_5);
           #endif
         }
       } else {
         __pyx_t_5 = __pyx_t_4(__pyx_t_2);
         if (unlikely(!__pyx_t_5)) {
           PyObject* exc_type = PyErr_Occurred();
           if (exc_type) {
             if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-            else __PYX_ERR(0, 864, __pyx_L5_error)
+            else __PYX_ERR(0, 879, __pyx_L5_error)
           }
           break;
         }
         __Pyx_GOTREF(__pyx_t_5);
       }
       __Pyx_XDECREF_SET(__pyx_8genexpr3__pyx_v_itm, __pyx_t_5);
       __pyx_t_5 = 0;
-      __pyx_t_5 = PySequence_List(__pyx_8genexpr3__pyx_v_itm); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 864, __pyx_L5_error)
+      __pyx_t_5 = PySequence_List(__pyx_8genexpr3__pyx_v_itm); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 879, __pyx_L5_error)
       __Pyx_GOTREF(__pyx_t_5);
-      if (unlikely(__Pyx_ListComp_Append(__pyx_t_1, (PyObject*)__pyx_t_5))) __PYX_ERR(0, 864, __pyx_L5_error)
+      if (unlikely(__Pyx_ListComp_Append(__pyx_t_1, (PyObject*)__pyx_t_5))) __PYX_ERR(0, 879, __pyx_L5_error)
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     }
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_8genexpr3__pyx_v_itm); __pyx_8genexpr3__pyx_v_itm = 0;
     goto __pyx_L9_exit_scope;
     __pyx_L5_error:;
     __Pyx_XDECREF(__pyx_8genexpr3__pyx_v_itm); __pyx_8genexpr3__pyx_v_itm = 0;
     goto __pyx_L1_error;
     __pyx_L9_exit_scope:;
   } /* exit inner scope */
-  __pyx_t_2 = PyTuple_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 864, __pyx_L1_error)
+  __pyx_t_2 = PyTuple_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 879, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_GIVEREF(__pyx_t_1);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_t_1)) __PYX_ERR(0, 864, __pyx_L1_error);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_t_1)) __PYX_ERR(0, 879, __pyx_L1_error);
   __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 864, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 879, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_7Fortuna_24CumulativeWeightedChoice_8__init___lambda2, 0, __pyx_n_s_CumulativeWeightedChoice___init_2, NULL, __pyx_n_s_Fortuna, __pyx_d, NULL); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 864, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_7Fortuna_24CumulativeWeightedChoice_8__init___lambda2, 0, __pyx_n_s_CumulativeWeightedChoice___init_2, NULL, __pyx_n_s_Fortuna, __pyx_d, NULL); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 879, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_key, __pyx_t_5) < 0) __PYX_ERR(0, 864, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_key, __pyx_t_5) < 0) __PYX_ERR(0, 879, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_t_5 = __Pyx_PyObject_Call(__pyx_builtin_sorted, __pyx_t_2, __pyx_t_1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 864, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_Call(__pyx_builtin_sorted, __pyx_t_2, __pyx_t_1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 879, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_v_data = __pyx_t_5;
   __pyx_t_5 = 0;
 
-  /* "Fortuna.pyx":865
+  /* "Fortuna.pyx":880
  *         self.flat = flat
  *         data = sorted([list(itm) for itm in weighted_table], key=lambda x: x[0])
  *         prev_weight = 0             # <<<<<<<<<<<<<<
  *         for w_pair in data:
  *             w_pair[0], prev_weight = w_pair[0] - prev_weight, w_pair[0]
  */
   __Pyx_INCREF(__pyx_int_0);
   __pyx_v_prev_weight = __pyx_int_0;
 
-  /* "Fortuna.pyx":866
+  /* "Fortuna.pyx":881
  *         data = sorted([list(itm) for itm in weighted_table], key=lambda x: x[0])
  *         prev_weight = 0
  *         for w_pair in data:             # <<<<<<<<<<<<<<
  *             w_pair[0], prev_weight = w_pair[0] - prev_weight, w_pair[0]
  *         optimized_data = sorted(data, key=lambda x: x[0], reverse=True)
  */
   if (likely(PyList_CheckExact(__pyx_v_data)) || PyTuple_CheckExact(__pyx_v_data)) {
     __pyx_t_5 = __pyx_v_data; __Pyx_INCREF(__pyx_t_5);
     __pyx_t_3 = 0;
     __pyx_t_4 = NULL;
   } else {
-    __pyx_t_3 = -1; __pyx_t_5 = PyObject_GetIter(__pyx_v_data); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 866, __pyx_L1_error)
+    __pyx_t_3 = -1; __pyx_t_5 = PyObject_GetIter(__pyx_v_data); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 881, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
-    __pyx_t_4 = __Pyx_PyObject_GetIterNextFunc(__pyx_t_5); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 866, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_GetIterNextFunc(__pyx_t_5); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 881, __pyx_L1_error)
   }
   for (;;) {
     if (likely(!__pyx_t_4)) {
       if (likely(PyList_CheckExact(__pyx_t_5))) {
         {
           Py_ssize_t __pyx_temp = __Pyx_PyList_GET_SIZE(__pyx_t_5);
           #if !CYTHON_ASSUME_SAFE_MACROS
-          if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 866, __pyx_L1_error)
+          if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 881, __pyx_L1_error)
           #endif
           if (__pyx_t_3 >= __pyx_temp) break;
         }
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_1 = PyList_GET_ITEM(__pyx_t_5, __pyx_t_3); __Pyx_INCREF(__pyx_t_1); __pyx_t_3++; if (unlikely((0 < 0))) __PYX_ERR(0, 866, __pyx_L1_error)
+        __pyx_t_1 = PyList_GET_ITEM(__pyx_t_5, __pyx_t_3); __Pyx_INCREF(__pyx_t_1); __pyx_t_3++; if (unlikely((0 < 0))) __PYX_ERR(0, 881, __pyx_L1_error)
         #else
-        __pyx_t_1 = __Pyx_PySequence_ITEM(__pyx_t_5, __pyx_t_3); __pyx_t_3++; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 866, __pyx_L1_error)
+        __pyx_t_1 = __Pyx_PySequence_ITEM(__pyx_t_5, __pyx_t_3); __pyx_t_3++; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 881, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_1);
         #endif
       } else {
         {
           Py_ssize_t __pyx_temp = __Pyx_PyTuple_GET_SIZE(__pyx_t_5);
           #if !CYTHON_ASSUME_SAFE_MACROS
-          if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 866, __pyx_L1_error)
+          if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 881, __pyx_L1_error)
           #endif
           if (__pyx_t_3 >= __pyx_temp) break;
         }
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_1 = PyTuple_GET_ITEM(__pyx_t_5, __pyx_t_3); __Pyx_INCREF(__pyx_t_1); __pyx_t_3++; if (unlikely((0 < 0))) __PYX_ERR(0, 866, __pyx_L1_error)
+        __pyx_t_1 = PyTuple_GET_ITEM(__pyx_t_5, __pyx_t_3); __Pyx_INCREF(__pyx_t_1); __pyx_t_3++; if (unlikely((0 < 0))) __PYX_ERR(0, 881, __pyx_L1_error)
         #else
-        __pyx_t_1 = __Pyx_PySequence_ITEM(__pyx_t_5, __pyx_t_3); __pyx_t_3++; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 866, __pyx_L1_error)
+        __pyx_t_1 = __Pyx_PySequence_ITEM(__pyx_t_5, __pyx_t_3); __pyx_t_3++; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 881, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_1);
         #endif
       }
     } else {
       __pyx_t_1 = __pyx_t_4(__pyx_t_5);
       if (unlikely(!__pyx_t_1)) {
         PyObject* exc_type = PyErr_Occurred();
         if (exc_type) {
           if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-          else __PYX_ERR(0, 866, __pyx_L1_error)
+          else __PYX_ERR(0, 881, __pyx_L1_error)
         }
         break;
       }
       __Pyx_GOTREF(__pyx_t_1);
     }
     __Pyx_XDECREF_SET(__pyx_v_w_pair, __pyx_t_1);
     __pyx_t_1 = 0;
 
-    /* "Fortuna.pyx":867
+    /* "Fortuna.pyx":882
  *         prev_weight = 0
  *         for w_pair in data:
  *             w_pair[0], prev_weight = w_pair[0] - prev_weight, w_pair[0]             # <<<<<<<<<<<<<<
  *         optimized_data = sorted(data, key=lambda x: x[0], reverse=True)
  *         cum_weight = 0
  */
-    __pyx_t_1 = __Pyx_GetItemInt(__pyx_v_w_pair, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 867, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_GetItemInt(__pyx_v_w_pair, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 882, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_2 = PyNumber_Subtract(__pyx_t_1, __pyx_v_prev_weight); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 867, __pyx_L1_error)
+    __pyx_t_2 = PyNumber_Subtract(__pyx_t_1, __pyx_v_prev_weight); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 882, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __pyx_t_1 = __Pyx_GetItemInt(__pyx_v_w_pair, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 867, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_GetItemInt(__pyx_v_w_pair, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 882, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    if (unlikely((__Pyx_SetItemInt(__pyx_v_w_pair, 0, __pyx_t_2, long, 1, __Pyx_PyInt_From_long, 0, 0, 1) < 0))) __PYX_ERR(0, 867, __pyx_L1_error)
+    if (unlikely((__Pyx_SetItemInt(__pyx_v_w_pair, 0, __pyx_t_2, long, 1, __Pyx_PyInt_From_long, 0, 0, 1) < 0))) __PYX_ERR(0, 882, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_DECREF_SET(__pyx_v_prev_weight, __pyx_t_1);
     __pyx_t_1 = 0;
 
-    /* "Fortuna.pyx":866
+    /* "Fortuna.pyx":881
  *         data = sorted([list(itm) for itm in weighted_table], key=lambda x: x[0])
  *         prev_weight = 0
  *         for w_pair in data:             # <<<<<<<<<<<<<<
  *             w_pair[0], prev_weight = w_pair[0] - prev_weight, w_pair[0]
  *         optimized_data = sorted(data, key=lambda x: x[0], reverse=True)
  */
   }
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
-  /* "Fortuna.pyx":868
+  /* "Fortuna.pyx":883
  *         for w_pair in data:
  *             w_pair[0], prev_weight = w_pair[0] - prev_weight, w_pair[0]
  *         optimized_data = sorted(data, key=lambda x: x[0], reverse=True)             # <<<<<<<<<<<<<<
  *         cum_weight = 0
  *         for w_pair in optimized_data:
  */
-  __pyx_t_5 = PyTuple_New(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 868, __pyx_L1_error)
+  __pyx_t_5 = PyTuple_New(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 883, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_INCREF(__pyx_v_data);
   __Pyx_GIVEREF(__pyx_v_data);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_v_data)) __PYX_ERR(0, 868, __pyx_L1_error);
-  __pyx_t_1 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 868, __pyx_L1_error)
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_v_data)) __PYX_ERR(0, 883, __pyx_L1_error);
+  __pyx_t_1 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 883, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_7Fortuna_24CumulativeWeightedChoice_8__init___1lambda3, 0, __pyx_n_s_CumulativeWeightedChoice___init_2, NULL, __pyx_n_s_Fortuna, __pyx_d, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 868, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_7Fortuna_24CumulativeWeightedChoice_8__init___1lambda3, 0, __pyx_n_s_CumulativeWeightedChoice___init_2, NULL, __pyx_n_s_Fortuna, __pyx_d, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 883, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_key, __pyx_t_2) < 0) __PYX_ERR(0, 868, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_key, __pyx_t_2) < 0) __PYX_ERR(0, 883, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_reverse, Py_True) < 0) __PYX_ERR(0, 868, __pyx_L1_error)
-  __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_sorted, __pyx_t_5, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 868, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_reverse, Py_True) < 0) __PYX_ERR(0, 883, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_sorted, __pyx_t_5, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 883, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_v_optimized_data = __pyx_t_2;
   __pyx_t_2 = 0;
 
-  /* "Fortuna.pyx":869
+  /* "Fortuna.pyx":884
  *             w_pair[0], prev_weight = w_pair[0] - prev_weight, w_pair[0]
  *         optimized_data = sorted(data, key=lambda x: x[0], reverse=True)
  *         cum_weight = 0             # <<<<<<<<<<<<<<
  *         for w_pair in optimized_data:
  *             cum_weight += w_pair[0]
  */
   __Pyx_INCREF(__pyx_int_0);
   __pyx_v_cum_weight = __pyx_int_0;
 
-  /* "Fortuna.pyx":870
+  /* "Fortuna.pyx":885
  *         optimized_data = sorted(data, key=lambda x: x[0], reverse=True)
  *         cum_weight = 0
  *         for w_pair in optimized_data:             # <<<<<<<<<<<<<<
  *             cum_weight += w_pair[0]
  *             w_pair[0] = cum_weight
  */
   if (likely(PyList_CheckExact(__pyx_v_optimized_data)) || PyTuple_CheckExact(__pyx_v_optimized_data)) {
     __pyx_t_2 = __pyx_v_optimized_data; __Pyx_INCREF(__pyx_t_2);
     __pyx_t_3 = 0;
     __pyx_t_4 = NULL;
   } else {
-    __pyx_t_3 = -1; __pyx_t_2 = PyObject_GetIter(__pyx_v_optimized_data); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 870, __pyx_L1_error)
+    __pyx_t_3 = -1; __pyx_t_2 = PyObject_GetIter(__pyx_v_optimized_data); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 885, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_4 = __Pyx_PyObject_GetIterNextFunc(__pyx_t_2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 870, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_GetIterNextFunc(__pyx_t_2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 885, __pyx_L1_error)
   }
   for (;;) {
     if (likely(!__pyx_t_4)) {
       if (likely(PyList_CheckExact(__pyx_t_2))) {
         {
           Py_ssize_t __pyx_temp = __Pyx_PyList_GET_SIZE(__pyx_t_2);
           #if !CYTHON_ASSUME_SAFE_MACROS
-          if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 870, __pyx_L1_error)
+          if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 885, __pyx_L1_error)
           #endif
           if (__pyx_t_3 >= __pyx_temp) break;
         }
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_1 = PyList_GET_ITEM(__pyx_t_2, __pyx_t_3); __Pyx_INCREF(__pyx_t_1); __pyx_t_3++; if (unlikely((0 < 0))) __PYX_ERR(0, 870, __pyx_L1_error)
+        __pyx_t_1 = PyList_GET_ITEM(__pyx_t_2, __pyx_t_3); __Pyx_INCREF(__pyx_t_1); __pyx_t_3++; if (unlikely((0 < 0))) __PYX_ERR(0, 885, __pyx_L1_error)
         #else
-        __pyx_t_1 = __Pyx_PySequence_ITEM(__pyx_t_2, __pyx_t_3); __pyx_t_3++; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 870, __pyx_L1_error)
+        __pyx_t_1 = __Pyx_PySequence_ITEM(__pyx_t_2, __pyx_t_3); __pyx_t_3++; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 885, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_1);
         #endif
       } else {
         {
           Py_ssize_t __pyx_temp = __Pyx_PyTuple_GET_SIZE(__pyx_t_2);
           #if !CYTHON_ASSUME_SAFE_MACROS
-          if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 870, __pyx_L1_error)
+          if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 885, __pyx_L1_error)
           #endif
           if (__pyx_t_3 >= __pyx_temp) break;
         }
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_1 = PyTuple_GET_ITEM(__pyx_t_2, __pyx_t_3); __Pyx_INCREF(__pyx_t_1); __pyx_t_3++; if (unlikely((0 < 0))) __PYX_ERR(0, 870, __pyx_L1_error)
+        __pyx_t_1 = PyTuple_GET_ITEM(__pyx_t_2, __pyx_t_3); __Pyx_INCREF(__pyx_t_1); __pyx_t_3++; if (unlikely((0 < 0))) __PYX_ERR(0, 885, __pyx_L1_error)
         #else
-        __pyx_t_1 = __Pyx_PySequence_ITEM(__pyx_t_2, __pyx_t_3); __pyx_t_3++; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 870, __pyx_L1_error)
+        __pyx_t_1 = __Pyx_PySequence_ITEM(__pyx_t_2, __pyx_t_3); __pyx_t_3++; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 885, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_1);
         #endif
       }
     } else {
       __pyx_t_1 = __pyx_t_4(__pyx_t_2);
       if (unlikely(!__pyx_t_1)) {
         PyObject* exc_type = PyErr_Occurred();
         if (exc_type) {
           if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-          else __PYX_ERR(0, 870, __pyx_L1_error)
+          else __PYX_ERR(0, 885, __pyx_L1_error)
         }
         break;
       }
       __Pyx_GOTREF(__pyx_t_1);
     }
     __Pyx_XDECREF_SET(__pyx_v_w_pair, __pyx_t_1);
     __pyx_t_1 = 0;
 
-    /* "Fortuna.pyx":871
+    /* "Fortuna.pyx":886
  *         cum_weight = 0
  *         for w_pair in optimized_data:
  *             cum_weight += w_pair[0]             # <<<<<<<<<<<<<<
  *             w_pair[0] = cum_weight
  *         self.max_weight = optimized_data[-1][0]
  */
-    __pyx_t_1 = __Pyx_GetItemInt(__pyx_v_w_pair, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 871, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_GetItemInt(__pyx_v_w_pair, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 886, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_5 = PyNumber_InPlaceAdd(__pyx_v_cum_weight, __pyx_t_1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 871, __pyx_L1_error)
+    __pyx_t_5 = PyNumber_InPlaceAdd(__pyx_v_cum_weight, __pyx_t_1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 886, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_DECREF_SET(__pyx_v_cum_weight, __pyx_t_5);
     __pyx_t_5 = 0;
 
-    /* "Fortuna.pyx":872
+    /* "Fortuna.pyx":887
  *         for w_pair in optimized_data:
  *             cum_weight += w_pair[0]
  *             w_pair[0] = cum_weight             # <<<<<<<<<<<<<<
  *         self.max_weight = optimized_data[-1][0]
  *         self.data = tuple(tuple(itm) for itm in optimized_data)
  */
-    if (unlikely((__Pyx_SetItemInt(__pyx_v_w_pair, 0, __pyx_v_cum_weight, long, 1, __Pyx_PyInt_From_long, 0, 0, 1) < 0))) __PYX_ERR(0, 872, __pyx_L1_error)
+    if (unlikely((__Pyx_SetItemInt(__pyx_v_w_pair, 0, __pyx_v_cum_weight, long, 1, __Pyx_PyInt_From_long, 0, 0, 1) < 0))) __PYX_ERR(0, 887, __pyx_L1_error)
 
-    /* "Fortuna.pyx":870
+    /* "Fortuna.pyx":885
  *         optimized_data = sorted(data, key=lambda x: x[0], reverse=True)
  *         cum_weight = 0
  *         for w_pair in optimized_data:             # <<<<<<<<<<<<<<
  *             cum_weight += w_pair[0]
  *             w_pair[0] = cum_weight
  */
   }
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "Fortuna.pyx":873
+  /* "Fortuna.pyx":888
  *             cum_weight += w_pair[0]
  *             w_pair[0] = cum_weight
  *         self.max_weight = optimized_data[-1][0]             # <<<<<<<<<<<<<<
  *         self.data = tuple(tuple(itm) for itm in optimized_data)
  * 
  */
-  __pyx_t_2 = __Pyx_GetItemInt(__pyx_v_optimized_data, -1L, long, 1, __Pyx_PyInt_From_long, 0, 1, 1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 873, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_GetItemInt(__pyx_v_optimized_data, -1L, long, 1, __Pyx_PyInt_From_long, 0, 1, 1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 888, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_5 = __Pyx_GetItemInt(__pyx_t_2, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 873, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_GetItemInt(__pyx_t_2, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 888, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_max_weight, __pyx_t_5) < 0) __PYX_ERR(0, 873, __pyx_L1_error)
+  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_max_weight, __pyx_t_5) < 0) __PYX_ERR(0, 888, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
-  /* "Fortuna.pyx":874
+  /* "Fortuna.pyx":889
  *             w_pair[0] = cum_weight
  *         self.max_weight = optimized_data[-1][0]
  *         self.data = tuple(tuple(itm) for itm in optimized_data)             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_t_5 = __pyx_pf_7Fortuna_24CumulativeWeightedChoice_8__init___2genexpr(NULL, __pyx_v_optimized_data); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 874, __pyx_L1_error)
+  __pyx_t_5 = __pyx_pf_7Fortuna_24CumulativeWeightedChoice_8__init___2genexpr(NULL, __pyx_v_optimized_data); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 889, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_2 = __Pyx_PySequence_Tuple(__pyx_t_5); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 874, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PySequence_Tuple(__pyx_t_5); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 889, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_data, __pyx_t_2) < 0) __PYX_ERR(0, 874, __pyx_L1_error)
+  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_data, __pyx_t_2) < 0) __PYX_ERR(0, 889, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "Fortuna.pyx":852
+  /* "Fortuna.pyx":867
  *     __slots__ = ("flat", "max_weight", "data")
  * 
  *     def __init__(self,             # <<<<<<<<<<<<<<
  *                  weighted_table: Iterable,
  *                  flat: bool = True):
  */
 
@@ -22940,15 +23505,15 @@
   __Pyx_XDECREF(__pyx_8genexpr3__pyx_v_itm);
   __Pyx_XDECREF(__pyx_gb_7Fortuna_24CumulativeWeightedChoice_8__init___4generator1);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "Fortuna.pyx":881
+/* "Fortuna.pyx":896
  *     MultiChoice: generates multiple choice style questions on the terminal. """
  * 
  *     def __init__(self,             # <<<<<<<<<<<<<<
  *                  query: str,
  *                  *,
  */
 
@@ -22993,25 +23558,25 @@
   __pyx_nargs = PyTuple_Size(__pyx_args); if (unlikely(__pyx_nargs < 0)) return NULL;
   #endif
   #endif
   __pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
   {
     PyObject **__pyx_pyargnames[] = {&__pyx_n_s_self,&__pyx_n_s_query,&__pyx_n_s_options,&__pyx_n_s_default,&__pyx_n_s_strict,&__pyx_n_s_cursor,0};
 
-    /* "Fortuna.pyx":884
+    /* "Fortuna.pyx":899
  *                  query: str,
  *                  *,
  *                  options: Iterable[str] = (),             # <<<<<<<<<<<<<<
  *                  default: str = "",
  *                  strict: bool = False,
  */
     values[2] = __Pyx_Arg_NewRef_FASTCALL(((PyObject *)((PyObject*)__pyx_empty_tuple)));
     values[3] = __Pyx_Arg_NewRef_FASTCALL(((PyObject*)((PyObject*)__pyx_kp_u__2)));
 
-    /* "Fortuna.pyx":886
+    /* "Fortuna.pyx":901
  *                  options: Iterable[str] = (),
  *                  default: str = "",
  *                  strict: bool = False,             # <<<<<<<<<<<<<<
  *                  cursor: str = ">>>"):
  *         """ Multiple Choice
  */
     values[4] = __Pyx_Arg_NewRef_FASTCALL(((PyObject *)((PyObject *)Py_False)));
@@ -23029,38 +23594,38 @@
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_self)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 881, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 896, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_query)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[1]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 881, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 896, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("__init__", 1, 2, 2, 1); __PYX_ERR(0, 881, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__init__", 1, 2, 2, 1); __PYX_ERR(0, 896, __pyx_L3_error)
         }
       }
       if (kw_args > 0 && likely(kw_args <= 4)) {
         Py_ssize_t index;
         for (index = 2; index < 6 && kw_args > 0; index++) {
           PyObject* value = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, *__pyx_pyargnames[index]);
           if (value) { values[index] = __Pyx_Arg_NewRef_FASTCALL(value); kw_args--; }
-          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 881, __pyx_L3_error)
+          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 896, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "__init__") < 0)) __PYX_ERR(0, 881, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "__init__") < 0)) __PYX_ERR(0, 896, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs != 2)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
       values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
     }
@@ -23069,34 +23634,34 @@
     __pyx_v_options = values[2];
     __pyx_v_default = ((PyObject*)values[3]);
     __pyx_v_strict = values[4];
     __pyx_v_cursor = ((PyObject*)values[5]);
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__init__", 1, 2, 2, __pyx_nargs); __PYX_ERR(0, 881, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__init__", 1, 2, 2, __pyx_nargs); __PYX_ERR(0, 896, __pyx_L3_error)
   __pyx_L6_skip:;
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_AddTraceback("Fortuna.MultiChoice.__init__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_query), (&PyUnicode_Type), 0, "query", 1))) __PYX_ERR(0, 882, __pyx_L1_error)
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_default), (&PyUnicode_Type), 0, "default", 1))) __PYX_ERR(0, 885, __pyx_L1_error)
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_cursor), (&PyUnicode_Type), 0, "cursor", 1))) __PYX_ERR(0, 887, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_query), (&PyUnicode_Type), 0, "query", 1))) __PYX_ERR(0, 897, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_default), (&PyUnicode_Type), 0, "default", 1))) __PYX_ERR(0, 900, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_cursor), (&PyUnicode_Type), 0, "cursor", 1))) __PYX_ERR(0, 902, __pyx_L1_error)
   __pyx_r = __pyx_pf_7Fortuna_11MultiChoice___init__(__pyx_self, __pyx_v_self, __pyx_v_query, __pyx_v_options, __pyx_v_default, __pyx_v_strict, __pyx_v_cursor);
 
-  /* "Fortuna.pyx":881
+  /* "Fortuna.pyx":896
  *     MultiChoice: generates multiple choice style questions on the terminal. """
  * 
  *     def __init__(self,             # <<<<<<<<<<<<<<
  *                  query: str,
  *                  *,
  */
 
@@ -23112,15 +23677,15 @@
     }
   }
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 static PyObject *__pyx_gb_7Fortuna_11MultiChoice_8__init___2generator2(__pyx_CoroutineObject *__pyx_generator, CYTHON_UNUSED PyThreadState *__pyx_tstate, PyObject *__pyx_sent_value); /* proto */
 
-/* "Fortuna.pyx":912
+/* "Fortuna.pyx":927
  *         self.choice_pack = (
  *             self.prompt,
  *             *(f"{k}. {v.title()}" for k, v in self.data.items()),             # <<<<<<<<<<<<<<
  *             self.cursor,
  *         )
  */
 
@@ -23132,23 +23697,23 @@
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("genexpr", 0);
   __pyx_cur_scope = (struct __pyx_obj_7Fortuna___pyx_scope_struct_3_genexpr *)__pyx_tp_new_7Fortuna___pyx_scope_struct_3_genexpr(__pyx_ptype_7Fortuna___pyx_scope_struct_3_genexpr, __pyx_empty_tuple, NULL);
   if (unlikely(!__pyx_cur_scope)) {
     __pyx_cur_scope = ((struct __pyx_obj_7Fortuna___pyx_scope_struct_3_genexpr *)Py_None);
     __Pyx_INCREF(Py_None);
-    __PYX_ERR(0, 912, __pyx_L1_error)
+    __PYX_ERR(0, 927, __pyx_L1_error)
   } else {
     __Pyx_GOTREF((PyObject *)__pyx_cur_scope);
   }
   __pyx_cur_scope->__pyx_genexpr_arg_0 = __pyx_genexpr_arg_0;
   __Pyx_INCREF(__pyx_cur_scope->__pyx_genexpr_arg_0);
   __Pyx_GIVEREF(__pyx_cur_scope->__pyx_genexpr_arg_0);
   {
-    __pyx_CoroutineObject *gen = __Pyx_Generator_New((__pyx_coroutine_body_t) __pyx_gb_7Fortuna_11MultiChoice_8__init___2generator2, NULL, (PyObject *) __pyx_cur_scope, __pyx_n_s_genexpr, __pyx_n_s_MultiChoice___init___locals_gene, __pyx_n_s_Fortuna); if (unlikely(!gen)) __PYX_ERR(0, 912, __pyx_L1_error)
+    __pyx_CoroutineObject *gen = __Pyx_Generator_New((__pyx_coroutine_body_t) __pyx_gb_7Fortuna_11MultiChoice_8__init___2generator2, NULL, (PyObject *) __pyx_cur_scope, __pyx_n_s_genexpr, __pyx_n_s_MultiChoice___init___locals_gene, __pyx_n_s_Fortuna); if (unlikely(!gen)) __PYX_ERR(0, 927, __pyx_L1_error)
     __Pyx_DECREF(__pyx_cur_scope);
     __Pyx_RefNannyFinishContext();
     return (PyObject *) gen;
   }
 
   /* function exit code */
   __pyx_L1_error:;
@@ -23184,56 +23749,56 @@
     case 0: goto __pyx_L3_first_run;
     case 1: goto __pyx_L6_resume_from_yield;
     default: /* CPython raises the right error here */
     __Pyx_RefNannyFinishContext();
     return NULL;
   }
   __pyx_L3_first_run:;
-  if (unlikely(!__pyx_sent_value)) __PYX_ERR(0, 912, __pyx_L1_error)
+  if (unlikely(!__pyx_sent_value)) __PYX_ERR(0, 927, __pyx_L1_error)
   __pyx_t_2 = 0;
-  if (unlikely(!__pyx_cur_scope->__pyx_genexpr_arg_0)) { __Pyx_RaiseUnboundLocalError(".0"); __PYX_ERR(0, 912, __pyx_L1_error) }
+  if (unlikely(!__pyx_cur_scope->__pyx_genexpr_arg_0)) { __Pyx_RaiseUnboundLocalError(".0"); __PYX_ERR(0, 927, __pyx_L1_error) }
   if (unlikely(__pyx_cur_scope->__pyx_genexpr_arg_0 == Py_None)) {
     PyErr_Format(PyExc_AttributeError, "'NoneType' object has no attribute '%.30s'", "items");
-    __PYX_ERR(0, 912, __pyx_L1_error)
+    __PYX_ERR(0, 927, __pyx_L1_error)
   }
-  __pyx_t_5 = __Pyx_dict_iterator(__pyx_cur_scope->__pyx_genexpr_arg_0, 0, __pyx_n_s_items, (&__pyx_t_3), (&__pyx_t_4)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 912, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_dict_iterator(__pyx_cur_scope->__pyx_genexpr_arg_0, 0, __pyx_n_s_items, (&__pyx_t_3), (&__pyx_t_4)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 927, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_XDECREF(__pyx_t_1);
   __pyx_t_1 = __pyx_t_5;
   __pyx_t_5 = 0;
   while (1) {
     __pyx_t_7 = __Pyx_dict_iter_next(__pyx_t_1, __pyx_t_3, &__pyx_t_2, &__pyx_t_5, &__pyx_t_6, NULL, __pyx_t_4);
     if (unlikely(__pyx_t_7 == 0)) break;
-    if (unlikely(__pyx_t_7 == -1)) __PYX_ERR(0, 912, __pyx_L1_error)
+    if (unlikely(__pyx_t_7 == -1)) __PYX_ERR(0, 927, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_GOTREF(__pyx_t_6);
     __Pyx_XGOTREF(__pyx_cur_scope->__pyx_v_k);
     __Pyx_XDECREF_SET(__pyx_cur_scope->__pyx_v_k, __pyx_t_5);
     __Pyx_GIVEREF(__pyx_t_5);
     __pyx_t_5 = 0;
     __Pyx_XGOTREF(__pyx_cur_scope->__pyx_v_v);
     __Pyx_XDECREF_SET(__pyx_cur_scope->__pyx_v_v, __pyx_t_6);
     __Pyx_GIVEREF(__pyx_t_6);
     __pyx_t_6 = 0;
-    __pyx_t_6 = PyTuple_New(3); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 912, __pyx_L1_error)
+    __pyx_t_6 = PyTuple_New(3); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 927, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __pyx_t_8 = 0;
     __pyx_t_9 = 127;
-    __pyx_t_5 = __Pyx_PyObject_FormatSimple(__pyx_cur_scope->__pyx_v_k, __pyx_empty_unicode); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 912, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyObject_FormatSimple(__pyx_cur_scope->__pyx_v_k, __pyx_empty_unicode); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 927, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __pyx_t_9 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_5) > __pyx_t_9) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_5) : __pyx_t_9;
     __pyx_t_8 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_5);
     __Pyx_GIVEREF(__pyx_t_5);
     PyTuple_SET_ITEM(__pyx_t_6, 0, __pyx_t_5);
     __pyx_t_5 = 0;
     __Pyx_INCREF(__pyx_kp_u__4);
     __pyx_t_8 += 2;
     __Pyx_GIVEREF(__pyx_kp_u__4);
     PyTuple_SET_ITEM(__pyx_t_6, 1, __pyx_kp_u__4);
-    __pyx_t_10 = __Pyx_PyObject_GetAttrStr(__pyx_cur_scope->__pyx_v_v, __pyx_n_s_title); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 912, __pyx_L1_error)
+    __pyx_t_10 = __Pyx_PyObject_GetAttrStr(__pyx_cur_scope->__pyx_v_v, __pyx_n_s_title); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 927, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_10);
     __pyx_t_11 = NULL;
     __pyx_t_7 = 0;
     #if CYTHON_UNPACK_METHODS
     if (likely(PyMethod_Check(__pyx_t_10))) {
       __pyx_t_11 = PyMethod_GET_SELF(__pyx_t_10);
       if (likely(__pyx_t_11)) {
@@ -23245,27 +23810,27 @@
       }
     }
     #endif
     {
       PyObject *__pyx_callargs[2] = {__pyx_t_11, NULL};
       __pyx_t_5 = __Pyx_PyObject_FastCall(__pyx_t_10, __pyx_callargs+1-__pyx_t_7, 0+__pyx_t_7);
       __Pyx_XDECREF(__pyx_t_11); __pyx_t_11 = 0;
-      if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 912, __pyx_L1_error)
+      if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 927, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
     }
-    __pyx_t_10 = __Pyx_PyObject_FormatSimple(__pyx_t_5, __pyx_empty_unicode); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 912, __pyx_L1_error)
+    __pyx_t_10 = __Pyx_PyObject_FormatSimple(__pyx_t_5, __pyx_empty_unicode); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 927, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_10);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     __pyx_t_9 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_10) > __pyx_t_9) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_10) : __pyx_t_9;
     __pyx_t_8 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_10);
     __Pyx_GIVEREF(__pyx_t_10);
     PyTuple_SET_ITEM(__pyx_t_6, 2, __pyx_t_10);
     __pyx_t_10 = 0;
-    __pyx_t_10 = __Pyx_PyUnicode_Join(__pyx_t_6, 3, __pyx_t_8, __pyx_t_9); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 912, __pyx_L1_error)
+    __pyx_t_10 = __Pyx_PyUnicode_Join(__pyx_t_6, 3, __pyx_t_8, __pyx_t_9); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 927, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_10);
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     __pyx_r = __pyx_t_10;
     __pyx_t_10 = 0;
     __Pyx_XGIVEREF(__pyx_t_1);
     __pyx_cur_scope->__pyx_t_0 = __pyx_t_1;
     __pyx_cur_scope->__pyx_t_1 = __pyx_t_2;
@@ -23280,15 +23845,15 @@
     __pyx_L6_resume_from_yield:;
     __pyx_t_1 = __pyx_cur_scope->__pyx_t_0;
     __pyx_cur_scope->__pyx_t_0 = 0;
     __Pyx_XGOTREF(__pyx_t_1);
     __pyx_t_2 = __pyx_cur_scope->__pyx_t_1;
     __pyx_t_3 = __pyx_cur_scope->__pyx_t_2;
     __pyx_t_4 = __pyx_cur_scope->__pyx_t_3;
-    if (unlikely(!__pyx_sent_value)) __PYX_ERR(0, 912, __pyx_L1_error)
+    if (unlikely(!__pyx_sent_value)) __PYX_ERR(0, 927, __pyx_L1_error)
   }
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   CYTHON_MAYBE_UNUSED_VAR(__pyx_cur_scope);
 
   /* function exit code */
   PyErr_SetNone(PyExc_StopIteration);
   goto __pyx_L0;
@@ -23307,15 +23872,15 @@
   #endif
   __pyx_generator->resume_label = -1;
   __Pyx_Coroutine_clear((PyObject*)__pyx_generator);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "Fortuna.pyx":881
+/* "Fortuna.pyx":896
  *     MultiChoice: generates multiple choice style questions on the terminal. """
  * 
  *     def __init__(self,             # <<<<<<<<<<<<<<
  *                  query: str,
  *                  *,
  */
 
@@ -23336,158 +23901,158 @@
   PyObject *__pyx_t_9 = NULL;
   int __pyx_t_10;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__init__", 1);
 
-  /* "Fortuna.pyx":902
+  /* "Fortuna.pyx":917
  *         @param cursor: Optional String. Default='>>>' Indicates user input.
  *         """
  *         self.cursor = cursor + ' '             # <<<<<<<<<<<<<<
  *         self.prompt = query
  *         self.options = tuple(options)
  */
-  __pyx_t_1 = __Pyx_PyUnicode_Concat(__pyx_v_cursor, __pyx_kp_u__5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 902, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyUnicode_Concat(__pyx_v_cursor, __pyx_kp_u__5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 917, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_cursor, __pyx_t_1) < 0) __PYX_ERR(0, 902, __pyx_L1_error)
+  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_cursor, __pyx_t_1) < 0) __PYX_ERR(0, 917, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "Fortuna.pyx":903
+  /* "Fortuna.pyx":918
  *         """
  *         self.cursor = cursor + ' '
  *         self.prompt = query             # <<<<<<<<<<<<<<
  *         self.options = tuple(options)
  *         self.default = default.lower()
  */
-  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_prompt, __pyx_v_query) < 0) __PYX_ERR(0, 903, __pyx_L1_error)
+  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_prompt, __pyx_v_query) < 0) __PYX_ERR(0, 918, __pyx_L1_error)
 
-  /* "Fortuna.pyx":904
+  /* "Fortuna.pyx":919
  *         self.cursor = cursor + ' '
  *         self.prompt = query
  *         self.options = tuple(options)             # <<<<<<<<<<<<<<
  *         self.default = default.lower()
  *         self.strict = strict
  */
-  __pyx_t_1 = __Pyx_PySequence_Tuple(__pyx_v_options); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 904, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PySequence_Tuple(__pyx_v_options); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 919, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_options, __pyx_t_1) < 0) __PYX_ERR(0, 904, __pyx_L1_error)
+  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_options, __pyx_t_1) < 0) __PYX_ERR(0, 919, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "Fortuna.pyx":905
+  /* "Fortuna.pyx":920
  *         self.prompt = query
  *         self.options = tuple(options)
  *         self.default = default.lower()             # <<<<<<<<<<<<<<
  *         self.strict = strict
  *         self.data = {
  */
-  __pyx_t_1 = __Pyx_CallUnboundCMethod0(&__pyx_umethod_PyUnicode_Type_lower, __pyx_v_default); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 905, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_CallUnboundCMethod0(&__pyx_umethod_PyUnicode_Type_lower, __pyx_v_default); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 920, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_default, __pyx_t_1) < 0) __PYX_ERR(0, 905, __pyx_L1_error)
+  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_default, __pyx_t_1) < 0) __PYX_ERR(0, 920, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "Fortuna.pyx":906
+  /* "Fortuna.pyx":921
  *         self.options = tuple(options)
  *         self.default = default.lower()
  *         self.strict = strict             # <<<<<<<<<<<<<<
  *         self.data = {
  *             str(k + 1): v.lower() for k, v in enumerate(self.options)
  */
-  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_strict, __pyx_v_strict) < 0) __PYX_ERR(0, 906, __pyx_L1_error)
+  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_strict, __pyx_v_strict) < 0) __PYX_ERR(0, 921, __pyx_L1_error)
 
-  /* "Fortuna.pyx":907
+  /* "Fortuna.pyx":922
  *         self.default = default.lower()
  *         self.strict = strict
  *         self.data = {             # <<<<<<<<<<<<<<
  *             str(k + 1): v.lower() for k, v in enumerate(self.options)
  *         }
  */
   { /* enter inner scope */
-    __pyx_t_1 = PyDict_New(); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 907, __pyx_L5_error)
+    __pyx_t_1 = PyDict_New(); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 922, __pyx_L5_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_INCREF(__pyx_int_0);
     __pyx_t_2 = __pyx_int_0;
 
-    /* "Fortuna.pyx":908
+    /* "Fortuna.pyx":923
  *         self.strict = strict
  *         self.data = {
  *             str(k + 1): v.lower() for k, v in enumerate(self.options)             # <<<<<<<<<<<<<<
  *         }
  *         self.choice_pack = (
  */
-    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_options); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 908, __pyx_L5_error)
+    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_options); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 923, __pyx_L5_error)
     __Pyx_GOTREF(__pyx_t_3);
     if (likely(PyList_CheckExact(__pyx_t_3)) || PyTuple_CheckExact(__pyx_t_3)) {
       __pyx_t_4 = __pyx_t_3; __Pyx_INCREF(__pyx_t_4);
       __pyx_t_5 = 0;
       __pyx_t_6 = NULL;
     } else {
-      __pyx_t_5 = -1; __pyx_t_4 = PyObject_GetIter(__pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 908, __pyx_L5_error)
+      __pyx_t_5 = -1; __pyx_t_4 = PyObject_GetIter(__pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 923, __pyx_L5_error)
       __Pyx_GOTREF(__pyx_t_4);
-      __pyx_t_6 = __Pyx_PyObject_GetIterNextFunc(__pyx_t_4); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 908, __pyx_L5_error)
+      __pyx_t_6 = __Pyx_PyObject_GetIterNextFunc(__pyx_t_4); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 923, __pyx_L5_error)
     }
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     for (;;) {
       if (likely(!__pyx_t_6)) {
         if (likely(PyList_CheckExact(__pyx_t_4))) {
           {
             Py_ssize_t __pyx_temp = __Pyx_PyList_GET_SIZE(__pyx_t_4);
             #if !CYTHON_ASSUME_SAFE_MACROS
-            if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 908, __pyx_L5_error)
+            if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 923, __pyx_L5_error)
             #endif
             if (__pyx_t_5 >= __pyx_temp) break;
           }
           #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-          __pyx_t_3 = PyList_GET_ITEM(__pyx_t_4, __pyx_t_5); __Pyx_INCREF(__pyx_t_3); __pyx_t_5++; if (unlikely((0 < 0))) __PYX_ERR(0, 908, __pyx_L5_error)
+          __pyx_t_3 = PyList_GET_ITEM(__pyx_t_4, __pyx_t_5); __Pyx_INCREF(__pyx_t_3); __pyx_t_5++; if (unlikely((0 < 0))) __PYX_ERR(0, 923, __pyx_L5_error)
           #else
-          __pyx_t_3 = __Pyx_PySequence_ITEM(__pyx_t_4, __pyx_t_5); __pyx_t_5++; if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 908, __pyx_L5_error)
+          __pyx_t_3 = __Pyx_PySequence_ITEM(__pyx_t_4, __pyx_t_5); __pyx_t_5++; if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 923, __pyx_L5_error)
           __Pyx_GOTREF(__pyx_t_3);
           #endif
         } else {
           {
             Py_ssize_t __pyx_temp = __Pyx_PyTuple_GET_SIZE(__pyx_t_4);
             #if !CYTHON_ASSUME_SAFE_MACROS
-            if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 908, __pyx_L5_error)
+            if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 923, __pyx_L5_error)
             #endif
             if (__pyx_t_5 >= __pyx_temp) break;
           }
           #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-          __pyx_t_3 = PyTuple_GET_ITEM(__pyx_t_4, __pyx_t_5); __Pyx_INCREF(__pyx_t_3); __pyx_t_5++; if (unlikely((0 < 0))) __PYX_ERR(0, 908, __pyx_L5_error)
+          __pyx_t_3 = PyTuple_GET_ITEM(__pyx_t_4, __pyx_t_5); __Pyx_INCREF(__pyx_t_3); __pyx_t_5++; if (unlikely((0 < 0))) __PYX_ERR(0, 923, __pyx_L5_error)
           #else
-          __pyx_t_3 = __Pyx_PySequence_ITEM(__pyx_t_4, __pyx_t_5); __pyx_t_5++; if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 908, __pyx_L5_error)
+          __pyx_t_3 = __Pyx_PySequence_ITEM(__pyx_t_4, __pyx_t_5); __pyx_t_5++; if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 923, __pyx_L5_error)
           __Pyx_GOTREF(__pyx_t_3);
           #endif
         }
       } else {
         __pyx_t_3 = __pyx_t_6(__pyx_t_4);
         if (unlikely(!__pyx_t_3)) {
           PyObject* exc_type = PyErr_Occurred();
           if (exc_type) {
             if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-            else __PYX_ERR(0, 908, __pyx_L5_error)
+            else __PYX_ERR(0, 923, __pyx_L5_error)
           }
           break;
         }
         __Pyx_GOTREF(__pyx_t_3);
       }
       __Pyx_XDECREF_SET(__pyx_8genexpr5__pyx_v_v, __pyx_t_3);
       __pyx_t_3 = 0;
       __Pyx_INCREF(__pyx_t_2);
       __Pyx_XDECREF_SET(__pyx_8genexpr5__pyx_v_k, __pyx_t_2);
-      __pyx_t_3 = __Pyx_PyInt_AddObjC(__pyx_t_2, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 908, __pyx_L5_error)
+      __pyx_t_3 = __Pyx_PyInt_AddObjC(__pyx_t_2, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 923, __pyx_L5_error)
       __Pyx_GOTREF(__pyx_t_3);
       __Pyx_DECREF(__pyx_t_2);
       __pyx_t_2 = __pyx_t_3;
       __pyx_t_3 = 0;
-      __pyx_t_3 = __Pyx_PyInt_AddObjC(__pyx_8genexpr5__pyx_v_k, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 908, __pyx_L5_error)
+      __pyx_t_3 = __Pyx_PyInt_AddObjC(__pyx_8genexpr5__pyx_v_k, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 923, __pyx_L5_error)
       __Pyx_GOTREF(__pyx_t_3);
-      __pyx_t_7 = __Pyx_PyObject_Str(__pyx_t_3); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 908, __pyx_L5_error)
+      __pyx_t_7 = __Pyx_PyObject_Str(__pyx_t_3); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 923, __pyx_L5_error)
       __Pyx_GOTREF(__pyx_t_7);
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_8genexpr5__pyx_v_v, __pyx_n_s_lower); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 908, __pyx_L5_error)
+      __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_8genexpr5__pyx_v_v, __pyx_n_s_lower); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 923, __pyx_L5_error)
       __Pyx_GOTREF(__pyx_t_8);
       __pyx_t_9 = NULL;
       __pyx_t_10 = 0;
       #if CYTHON_UNPACK_METHODS
       if (likely(PyMethod_Check(__pyx_t_8))) {
         __pyx_t_9 = PyMethod_GET_SELF(__pyx_t_8);
         if (likely(__pyx_t_9)) {
@@ -23499,19 +24064,19 @@
         }
       }
       #endif
       {
         PyObject *__pyx_callargs[2] = {__pyx_t_9, NULL};
         __pyx_t_3 = __Pyx_PyObject_FastCall(__pyx_t_8, __pyx_callargs+1-__pyx_t_10, 0+__pyx_t_10);
         __Pyx_XDECREF(__pyx_t_9); __pyx_t_9 = 0;
-        if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 908, __pyx_L5_error)
+        if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 923, __pyx_L5_error)
         __Pyx_GOTREF(__pyx_t_3);
         __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       }
-      if (unlikely(PyDict_SetItem(__pyx_t_1, (PyObject*)__pyx_t_7, (PyObject*)__pyx_t_3))) __PYX_ERR(0, 908, __pyx_L5_error)
+      if (unlikely(PyDict_SetItem(__pyx_t_1, (PyObject*)__pyx_t_7, (PyObject*)__pyx_t_3))) __PYX_ERR(0, 923, __pyx_L5_error)
       __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     }
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_8genexpr5__pyx_v_k); __pyx_8genexpr5__pyx_v_k = 0;
     __Pyx_XDECREF(__pyx_8genexpr5__pyx_v_v); __pyx_8genexpr5__pyx_v_v = 0;
@@ -23519,85 +24084,85 @@
     __pyx_L5_error:;
     __Pyx_XDECREF(__pyx_8genexpr5__pyx_v_k); __pyx_8genexpr5__pyx_v_k = 0;
     __Pyx_XDECREF(__pyx_8genexpr5__pyx_v_v); __pyx_8genexpr5__pyx_v_v = 0;
     goto __pyx_L1_error;
     __pyx_L9_exit_scope:;
   } /* exit inner scope */
 
-  /* "Fortuna.pyx":907
+  /* "Fortuna.pyx":922
  *         self.default = default.lower()
  *         self.strict = strict
  *         self.data = {             # <<<<<<<<<<<<<<
  *             str(k + 1): v.lower() for k, v in enumerate(self.options)
  *         }
  */
-  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_data, __pyx_t_1) < 0) __PYX_ERR(0, 907, __pyx_L1_error)
+  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_data, __pyx_t_1) < 0) __PYX_ERR(0, 922, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "Fortuna.pyx":911
+  /* "Fortuna.pyx":926
  *         }
  *         self.choice_pack = (
  *             self.prompt,             # <<<<<<<<<<<<<<
  *             *(f"{k}. {v.title()}" for k, v in self.data.items()),
  *             self.cursor,
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_prompt); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 911, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_prompt); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 926, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_4 = PyList_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 911, __pyx_L1_error)
+  __pyx_t_4 = PyList_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 926, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_GIVEREF(__pyx_t_2);
-  if (__Pyx_PyList_SET_ITEM(__pyx_t_4, 0, __pyx_t_2)) __PYX_ERR(0, 911, __pyx_L1_error);
+  if (__Pyx_PyList_SET_ITEM(__pyx_t_4, 0, __pyx_t_2)) __PYX_ERR(0, 926, __pyx_L1_error);
   __pyx_t_2 = 0;
   __pyx_t_1 = __pyx_t_4;
   __pyx_t_4 = 0;
 
-  /* "Fortuna.pyx":912
+  /* "Fortuna.pyx":927
  *         self.choice_pack = (
  *             self.prompt,
  *             *(f"{k}. {v.title()}" for k, v in self.data.items()),             # <<<<<<<<<<<<<<
  *             self.cursor,
  *         )
  */
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_data); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 912, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_data); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 927, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_2 = __pyx_pf_7Fortuna_11MultiChoice_8__init___genexpr(NULL, __pyx_t_4); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 912, __pyx_L1_error)
+  __pyx_t_2 = __pyx_pf_7Fortuna_11MultiChoice_8__init___genexpr(NULL, __pyx_t_4); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 927, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (__Pyx_PyList_Extend(__pyx_t_1, __pyx_t_2) < 0) __PYX_ERR(0, 912, __pyx_L1_error)
+  if (__Pyx_PyList_Extend(__pyx_t_1, __pyx_t_2) < 0) __PYX_ERR(0, 927, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "Fortuna.pyx":913
+  /* "Fortuna.pyx":928
  *             self.prompt,
  *             *(f"{k}. {v.title()}" for k, v in self.data.items()),
  *             self.cursor,             # <<<<<<<<<<<<<<
  *         )
  * 
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_cursor); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 913, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_cursor); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 928, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (__Pyx_ListComp_Append(__pyx_t_1, __pyx_t_2) < 0) __PYX_ERR(0, 913, __pyx_L1_error)
+  if (__Pyx_ListComp_Append(__pyx_t_1, __pyx_t_2) < 0) __PYX_ERR(0, 928, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   {
     PyObject *__pyx_temp = PyList_AsTuple(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_1);
-    __pyx_t_1 = __pyx_temp; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 911, __pyx_L1_error)
+    __pyx_t_1 = __pyx_temp; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 926, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
   }
 
-  /* "Fortuna.pyx":910
+  /* "Fortuna.pyx":925
  *             str(k + 1): v.lower() for k, v in enumerate(self.options)
  *         }
  *         self.choice_pack = (             # <<<<<<<<<<<<<<
  *             self.prompt,
  *             *(f"{k}. {v.title()}" for k, v in self.data.items()),
  */
-  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_choice_pack, __pyx_t_1) < 0) __PYX_ERR(0, 910, __pyx_L1_error)
+  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_choice_pack, __pyx_t_1) < 0) __PYX_ERR(0, 925, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "Fortuna.pyx":881
+  /* "Fortuna.pyx":896
  *     MultiChoice: generates multiple choice style questions on the terminal. """
  * 
  *     def __init__(self,             # <<<<<<<<<<<<<<
  *                  query: str,
  *                  *,
  */
 
@@ -23619,15 +24184,15 @@
   __Pyx_XDECREF(__pyx_8genexpr5__pyx_v_v);
   __Pyx_XDECREF(__pyx_gb_7Fortuna_11MultiChoice_8__init___2generator2);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "Fortuna.pyx":916
+/* "Fortuna.pyx":931
  *         )
  * 
  *     def _get_answer(self) -> str:             # <<<<<<<<<<<<<<
  *         return input('\n'.join(self.choice_pack)).lower() or self.default
  * 
  */
 
@@ -23681,31 +24246,31 @@
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_self)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 916, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 931, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "_get_answer") < 0)) __PYX_ERR(0, 916, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "_get_answer") < 0)) __PYX_ERR(0, 931, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs != 1)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
     }
     __pyx_v_self = values[0];
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("_get_answer", 1, 1, 1, __pyx_nargs); __PYX_ERR(0, 916, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("_get_answer", 1, 1, 1, __pyx_nargs); __PYX_ERR(0, 931, __pyx_L3_error)
   __pyx_L6_skip:;
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
@@ -23738,31 +24303,31 @@
   int __pyx_t_5;
   int __pyx_t_6;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_get_answer", 1);
 
-  /* "Fortuna.pyx":917
+  /* "Fortuna.pyx":932
  * 
  *     def _get_answer(self) -> str:
  *         return input('\n'.join(self.choice_pack)).lower() or self.default             # <<<<<<<<<<<<<<
  * 
  *     def __call__(self) -> str:
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_choice_pack); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 917, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_choice_pack); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 932, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = PyUnicode_Join(__pyx_kp_u__6, __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 917, __pyx_L1_error)
+  __pyx_t_4 = PyUnicode_Join(__pyx_kp_u__6, __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 932, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_PyObject_CallOneArg(__pyx_builtin_input, __pyx_t_4); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 917, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_CallOneArg(__pyx_builtin_input, __pyx_t_4); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 932, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_lower); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 917, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_lower); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 932, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_t_3 = NULL;
   __pyx_t_5 = 0;
   #if CYTHON_UNPACK_METHODS
   if (likely(PyMethod_Check(__pyx_t_4))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_4);
@@ -23775,40 +24340,40 @@
     }
   }
   #endif
   {
     PyObject *__pyx_callargs[2] = {__pyx_t_3, NULL};
     __pyx_t_2 = __Pyx_PyObject_FastCall(__pyx_t_4, __pyx_callargs+1-__pyx_t_5, 0+__pyx_t_5);
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 917, __pyx_L1_error)
+    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 932, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   }
-  __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely((__pyx_t_6 < 0))) __PYX_ERR(0, 917, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely((__pyx_t_6 < 0))) __PYX_ERR(0, 932, __pyx_L1_error)
   if (!__pyx_t_6) {
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   } else {
-    if (!(likely(PyUnicode_CheckExact(__pyx_t_2))||((__pyx_t_2) == Py_None) || __Pyx_RaiseUnexpectedTypeError("unicode", __pyx_t_2))) __PYX_ERR(0, 917, __pyx_L1_error)
+    if (!(likely(PyUnicode_CheckExact(__pyx_t_2))||((__pyx_t_2) == Py_None) || __Pyx_RaiseUnexpectedTypeError("unicode", __pyx_t_2))) __PYX_ERR(0, 932, __pyx_L1_error)
     __Pyx_INCREF(__pyx_t_2);
     __pyx_t_1 = __pyx_t_2;
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     goto __pyx_L3_bool_binop_done;
   }
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_default); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 917, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_default); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 932, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (!(likely(PyUnicode_CheckExact(__pyx_t_2))||((__pyx_t_2) == Py_None) || __Pyx_RaiseUnexpectedTypeError("unicode", __pyx_t_2))) __PYX_ERR(0, 917, __pyx_L1_error)
+  if (!(likely(PyUnicode_CheckExact(__pyx_t_2))||((__pyx_t_2) == Py_None) || __Pyx_RaiseUnexpectedTypeError("unicode", __pyx_t_2))) __PYX_ERR(0, 932, __pyx_L1_error)
   __Pyx_INCREF(__pyx_t_2);
   __pyx_t_1 = __pyx_t_2;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_L3_bool_binop_done:;
   __pyx_r = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "Fortuna.pyx":916
+  /* "Fortuna.pyx":931
  *         )
  * 
  *     def _get_answer(self) -> str:             # <<<<<<<<<<<<<<
  *         return input('\n'.join(self.choice_pack)).lower() or self.default
  * 
  */
 
@@ -23822,15 +24387,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "Fortuna.pyx":919
+/* "Fortuna.pyx":934
  *         return input('\n'.join(self.choice_pack)).lower() or self.default
  * 
  *     def __call__(self) -> str:             # <<<<<<<<<<<<<<
  *         """ @return: String. Returns the user's selection. """
  *         selection = self._get_answer()
  */
 
@@ -23884,31 +24449,31 @@
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_self)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 919, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 934, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "__call__") < 0)) __PYX_ERR(0, 919, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "__call__") < 0)) __PYX_ERR(0, 934, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs != 1)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
     }
     __pyx_v_self = values[0];
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__call__", 1, 1, 1, __pyx_nargs); __PYX_ERR(0, 919, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__call__", 1, 1, 1, __pyx_nargs); __PYX_ERR(0, 934, __pyx_L3_error)
   __pyx_L6_skip:;
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
@@ -23944,22 +24509,22 @@
   int __pyx_t_7;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__call__", 1);
 
-  /* "Fortuna.pyx":921
+  /* "Fortuna.pyx":936
  *     def __call__(self) -> str:
  *         """ @return: String. Returns the user's selection. """
  *         selection = self._get_answer()             # <<<<<<<<<<<<<<
  *         if not selection and self.options:
  *             return random_value(self.options)
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_get_answer); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 921, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_get_answer); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 936, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
   __pyx_t_4 = 0;
   #if CYTHON_UNPACK_METHODS
   if (likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
@@ -23971,54 +24536,54 @@
     }
   }
   #endif
   {
     PyObject *__pyx_callargs[2] = {__pyx_t_3, NULL};
     __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_2, __pyx_callargs+1-__pyx_t_4, 0+__pyx_t_4);
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 921, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 936, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   }
   __pyx_v_selection = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "Fortuna.pyx":922
+  /* "Fortuna.pyx":937
  *         """ @return: String. Returns the user's selection. """
  *         selection = self._get_answer()
  *         if not selection and self.options:             # <<<<<<<<<<<<<<
  *             return random_value(self.options)
  *         elif selection in self.data.values():
  */
-  __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_v_selection); if (unlikely((__pyx_t_6 < 0))) __PYX_ERR(0, 922, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_v_selection); if (unlikely((__pyx_t_6 < 0))) __PYX_ERR(0, 937, __pyx_L1_error)
   __pyx_t_7 = (!__pyx_t_6);
   if (__pyx_t_7) {
   } else {
     __pyx_t_5 = __pyx_t_7;
     goto __pyx_L4_bool_binop_done;
   }
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_options); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 922, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_options); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 937, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_7 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely((__pyx_t_7 < 0))) __PYX_ERR(0, 922, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely((__pyx_t_7 < 0))) __PYX_ERR(0, 937, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_5 = __pyx_t_7;
   __pyx_L4_bool_binop_done:;
   if (__pyx_t_5) {
 
-    /* "Fortuna.pyx":923
+    /* "Fortuna.pyx":938
  *         selection = self._get_answer()
  *         if not selection and self.options:
  *             return random_value(self.options)             # <<<<<<<<<<<<<<
  *         elif selection in self.data.values():
  *             return selection.title()
  */
     __Pyx_XDECREF(__pyx_r);
-    __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_random_value); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 923, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_random_value); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 938, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_options); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 923, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_options); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 938, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __pyx_t_8 = NULL;
     __pyx_t_4 = 0;
     #if CYTHON_UNPACK_METHODS
     if (unlikely(PyMethod_Check(__pyx_t_2))) {
       __pyx_t_8 = PyMethod_GET_SELF(__pyx_t_2);
       if (likely(__pyx_t_8)) {
@@ -24031,42 +24596,42 @@
     }
     #endif
     {
       PyObject *__pyx_callargs[2] = {__pyx_t_8, __pyx_t_3};
       __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_2, __pyx_callargs+1-__pyx_t_4, 1+__pyx_t_4);
       __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 923, __pyx_L1_error)
+      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 938, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     }
-    if (!(likely(PyUnicode_CheckExact(__pyx_t_1))||((__pyx_t_1) == Py_None) || __Pyx_RaiseUnexpectedTypeError("unicode", __pyx_t_1))) __PYX_ERR(0, 923, __pyx_L1_error)
+    if (!(likely(PyUnicode_CheckExact(__pyx_t_1))||((__pyx_t_1) == Py_None) || __Pyx_RaiseUnexpectedTypeError("unicode", __pyx_t_1))) __PYX_ERR(0, 938, __pyx_L1_error)
     __pyx_r = ((PyObject*)__pyx_t_1);
     __pyx_t_1 = 0;
     goto __pyx_L0;
 
-    /* "Fortuna.pyx":922
+    /* "Fortuna.pyx":937
  *         """ @return: String. Returns the user's selection. """
  *         selection = self._get_answer()
  *         if not selection and self.options:             # <<<<<<<<<<<<<<
  *             return random_value(self.options)
  *         elif selection in self.data.values():
  */
   }
 
-  /* "Fortuna.pyx":924
+  /* "Fortuna.pyx":939
  *         if not selection and self.options:
  *             return random_value(self.options)
  *         elif selection in self.data.values():             # <<<<<<<<<<<<<<
  *             return selection.title()
  *         elif selection in self.data.keys():
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_data); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 924, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_data); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 939, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_values); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 924, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_values); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 939, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_t_2 = NULL;
   __pyx_t_4 = 0;
   #if CYTHON_UNPACK_METHODS
   if (likely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_3);
@@ -24079,31 +24644,31 @@
     }
   }
   #endif
   {
     PyObject *__pyx_callargs[2] = {__pyx_t_2, NULL};
     __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_4, 0+__pyx_t_4);
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 924, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 939, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   }
-  __pyx_t_5 = (__Pyx_PySequence_ContainsTF(__pyx_v_selection, __pyx_t_1, Py_EQ)); if (unlikely((__pyx_t_5 < 0))) __PYX_ERR(0, 924, __pyx_L1_error)
+  __pyx_t_5 = (__Pyx_PySequence_ContainsTF(__pyx_v_selection, __pyx_t_1, Py_EQ)); if (unlikely((__pyx_t_5 < 0))) __PYX_ERR(0, 939, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   if (__pyx_t_5) {
 
-    /* "Fortuna.pyx":925
+    /* "Fortuna.pyx":940
  *             return random_value(self.options)
  *         elif selection in self.data.values():
  *             return selection.title()             # <<<<<<<<<<<<<<
  *         elif selection in self.data.keys():
  *             return self.data[selection].title()
  */
     __Pyx_XDECREF(__pyx_r);
-    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_selection, __pyx_n_s_title); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 925, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_selection, __pyx_n_s_title); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 940, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __pyx_t_2 = NULL;
     __pyx_t_4 = 0;
     #if CYTHON_UNPACK_METHODS
     if (likely(PyMethod_Check(__pyx_t_3))) {
       __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_3);
       if (likely(__pyx_t_2)) {
@@ -24115,42 +24680,42 @@
       }
     }
     #endif
     {
       PyObject *__pyx_callargs[2] = {__pyx_t_2, NULL};
       __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_4, 0+__pyx_t_4);
       __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
-      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 925, __pyx_L1_error)
+      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 940, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     }
-    if (!(likely(PyUnicode_CheckExact(__pyx_t_1))||((__pyx_t_1) == Py_None) || __Pyx_RaiseUnexpectedTypeError("unicode", __pyx_t_1))) __PYX_ERR(0, 925, __pyx_L1_error)
+    if (!(likely(PyUnicode_CheckExact(__pyx_t_1))||((__pyx_t_1) == Py_None) || __Pyx_RaiseUnexpectedTypeError("unicode", __pyx_t_1))) __PYX_ERR(0, 940, __pyx_L1_error)
     __pyx_r = ((PyObject*)__pyx_t_1);
     __pyx_t_1 = 0;
     goto __pyx_L0;
 
-    /* "Fortuna.pyx":924
+    /* "Fortuna.pyx":939
  *         if not selection and self.options:
  *             return random_value(self.options)
  *         elif selection in self.data.values():             # <<<<<<<<<<<<<<
  *             return selection.title()
  *         elif selection in self.data.keys():
  */
   }
 
-  /* "Fortuna.pyx":926
+  /* "Fortuna.pyx":941
  *         elif selection in self.data.values():
  *             return selection.title()
  *         elif selection in self.data.keys():             # <<<<<<<<<<<<<<
  *             return self.data[selection].title()
  *         elif selection and not self.strict:
  */
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_data); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 926, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_data); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 941, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_keys); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 926, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_keys); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 941, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_t_3 = NULL;
   __pyx_t_4 = 0;
   #if CYTHON_UNPACK_METHODS
   if (likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
@@ -24163,36 +24728,36 @@
     }
   }
   #endif
   {
     PyObject *__pyx_callargs[2] = {__pyx_t_3, NULL};
     __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_2, __pyx_callargs+1-__pyx_t_4, 0+__pyx_t_4);
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 926, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 941, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   }
-  __pyx_t_5 = (__Pyx_PySequence_ContainsTF(__pyx_v_selection, __pyx_t_1, Py_EQ)); if (unlikely((__pyx_t_5 < 0))) __PYX_ERR(0, 926, __pyx_L1_error)
+  __pyx_t_5 = (__Pyx_PySequence_ContainsTF(__pyx_v_selection, __pyx_t_1, Py_EQ)); if (unlikely((__pyx_t_5 < 0))) __PYX_ERR(0, 941, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   if (__pyx_t_5) {
 
-    /* "Fortuna.pyx":927
+    /* "Fortuna.pyx":942
  *             return selection.title()
  *         elif selection in self.data.keys():
  *             return self.data[selection].title()             # <<<<<<<<<<<<<<
  *         elif selection and not self.strict:
  *             return selection.title()
  */
     __Pyx_XDECREF(__pyx_r);
-    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_data); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 927, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_data); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 942, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_3 = __Pyx_PyObject_GetItem(__pyx_t_2, __pyx_v_selection); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 927, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_GetItem(__pyx_t_2, __pyx_v_selection); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 942, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_title); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 927, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_title); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 942, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __pyx_t_3 = NULL;
     __pyx_t_4 = 0;
     #if CYTHON_UNPACK_METHODS
     if (likely(PyMethod_Check(__pyx_t_2))) {
       __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
@@ -24205,63 +24770,63 @@
       }
     }
     #endif
     {
       PyObject *__pyx_callargs[2] = {__pyx_t_3, NULL};
       __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_2, __pyx_callargs+1-__pyx_t_4, 0+__pyx_t_4);
       __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 927, __pyx_L1_error)
+      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 942, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     }
-    if (!(likely(PyUnicode_CheckExact(__pyx_t_1))||((__pyx_t_1) == Py_None) || __Pyx_RaiseUnexpectedTypeError("unicode", __pyx_t_1))) __PYX_ERR(0, 927, __pyx_L1_error)
+    if (!(likely(PyUnicode_CheckExact(__pyx_t_1))||((__pyx_t_1) == Py_None) || __Pyx_RaiseUnexpectedTypeError("unicode", __pyx_t_1))) __PYX_ERR(0, 942, __pyx_L1_error)
     __pyx_r = ((PyObject*)__pyx_t_1);
     __pyx_t_1 = 0;
     goto __pyx_L0;
 
-    /* "Fortuna.pyx":926
+    /* "Fortuna.pyx":941
  *         elif selection in self.data.values():
  *             return selection.title()
  *         elif selection in self.data.keys():             # <<<<<<<<<<<<<<
  *             return self.data[selection].title()
  *         elif selection and not self.strict:
  */
   }
 
-  /* "Fortuna.pyx":928
+  /* "Fortuna.pyx":943
  *         elif selection in self.data.keys():
  *             return self.data[selection].title()
  *         elif selection and not self.strict:             # <<<<<<<<<<<<<<
  *             return selection.title()
  *         else:
  */
-  __pyx_t_7 = __Pyx_PyObject_IsTrue(__pyx_v_selection); if (unlikely((__pyx_t_7 < 0))) __PYX_ERR(0, 928, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyObject_IsTrue(__pyx_v_selection); if (unlikely((__pyx_t_7 < 0))) __PYX_ERR(0, 943, __pyx_L1_error)
   if (__pyx_t_7) {
   } else {
     __pyx_t_5 = __pyx_t_7;
     goto __pyx_L6_bool_binop_done;
   }
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_strict); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 928, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_strict); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 943, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_7 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely((__pyx_t_7 < 0))) __PYX_ERR(0, 928, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely((__pyx_t_7 < 0))) __PYX_ERR(0, 943, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_6 = (!__pyx_t_7);
   __pyx_t_5 = __pyx_t_6;
   __pyx_L6_bool_binop_done:;
   if (__pyx_t_5) {
 
-    /* "Fortuna.pyx":929
+    /* "Fortuna.pyx":944
  *             return self.data[selection].title()
  *         elif selection and not self.strict:
  *             return selection.title()             # <<<<<<<<<<<<<<
  *         else:
  *             return self()
  */
     __Pyx_XDECREF(__pyx_r);
-    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_selection, __pyx_n_s_title); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 929, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_selection, __pyx_n_s_title); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 944, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __pyx_t_3 = NULL;
     __pyx_t_4 = 0;
     #if CYTHON_UNPACK_METHODS
     if (likely(PyMethod_Check(__pyx_t_2))) {
       __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
       if (likely(__pyx_t_3)) {
@@ -24273,33 +24838,33 @@
       }
     }
     #endif
     {
       PyObject *__pyx_callargs[2] = {__pyx_t_3, NULL};
       __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_2, __pyx_callargs+1-__pyx_t_4, 0+__pyx_t_4);
       __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 929, __pyx_L1_error)
+      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 944, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     }
-    if (!(likely(PyUnicode_CheckExact(__pyx_t_1))||((__pyx_t_1) == Py_None) || __Pyx_RaiseUnexpectedTypeError("unicode", __pyx_t_1))) __PYX_ERR(0, 929, __pyx_L1_error)
+    if (!(likely(PyUnicode_CheckExact(__pyx_t_1))||((__pyx_t_1) == Py_None) || __Pyx_RaiseUnexpectedTypeError("unicode", __pyx_t_1))) __PYX_ERR(0, 944, __pyx_L1_error)
     __pyx_r = ((PyObject*)__pyx_t_1);
     __pyx_t_1 = 0;
     goto __pyx_L0;
 
-    /* "Fortuna.pyx":928
+    /* "Fortuna.pyx":943
  *         elif selection in self.data.keys():
  *             return self.data[selection].title()
  *         elif selection and not self.strict:             # <<<<<<<<<<<<<<
  *             return selection.title()
  *         else:
  */
   }
 
-  /* "Fortuna.pyx":931
+  /* "Fortuna.pyx":946
  *             return selection.title()
  *         else:
  *             return self()             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*else*/ {
@@ -24319,25 +24884,25 @@
       }
     }
     #endif
     {
       PyObject *__pyx_callargs[2] = {__pyx_t_3, NULL};
       __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_2, __pyx_callargs+1-__pyx_t_4, 0+__pyx_t_4);
       __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 931, __pyx_L1_error)
+      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 946, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     }
-    if (!(likely(PyUnicode_CheckExact(__pyx_t_1))||((__pyx_t_1) == Py_None) || __Pyx_RaiseUnexpectedTypeError("unicode", __pyx_t_1))) __PYX_ERR(0, 931, __pyx_L1_error)
+    if (!(likely(PyUnicode_CheckExact(__pyx_t_1))||((__pyx_t_1) == Py_None) || __Pyx_RaiseUnexpectedTypeError("unicode", __pyx_t_1))) __PYX_ERR(0, 946, __pyx_L1_error)
     __pyx_r = ((PyObject*)__pyx_t_1);
     __pyx_t_1 = 0;
     goto __pyx_L0;
   }
 
-  /* "Fortuna.pyx":919
+  /* "Fortuna.pyx":934
  *         return input('\n'.join(self.choice_pack)).lower() or self.default
  * 
  *     def __call__(self) -> str:             # <<<<<<<<<<<<<<
  *         """ @return: String. Returns the user's selection. """
  *         selection = self._get_answer()
  */
 
@@ -24352,15 +24917,15 @@
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_selection);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "Fortuna.pyx":934
+/* "Fortuna.pyx":949
  * 
  * 
  * def beta_variate(alpha: float, beta: float) -> float:             # <<<<<<<<<<<<<<
  *     return _beta(alpha, beta)
  * 
  */
 
@@ -24417,43 +24982,43 @@
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_alpha)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 934, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 949, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_beta)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[1]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 934, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 949, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("beta_variate", 1, 2, 2, 1); __PYX_ERR(0, 934, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("beta_variate", 1, 2, 2, 1); __PYX_ERR(0, 949, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "beta_variate") < 0)) __PYX_ERR(0, 934, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "beta_variate") < 0)) __PYX_ERR(0, 949, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs != 2)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
       values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
     }
-    __pyx_v_alpha = __pyx_PyFloat_AsDouble(values[0]); if (unlikely((__pyx_v_alpha == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 934, __pyx_L3_error)
-    __pyx_v_beta = __pyx_PyFloat_AsDouble(values[1]); if (unlikely((__pyx_v_beta == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 934, __pyx_L3_error)
+    __pyx_v_alpha = __pyx_PyFloat_AsDouble(values[0]); if (unlikely((__pyx_v_alpha == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 949, __pyx_L3_error)
+    __pyx_v_beta = __pyx_PyFloat_AsDouble(values[1]); if (unlikely((__pyx_v_beta == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 949, __pyx_L3_error)
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("beta_variate", 1, 2, 2, __pyx_nargs); __PYX_ERR(0, 934, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("beta_variate", 1, 2, 2, __pyx_nargs); __PYX_ERR(0, 949, __pyx_L3_error)
   __pyx_L6_skip:;
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
@@ -24481,29 +25046,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("beta_variate", 1);
 
-  /* "Fortuna.pyx":935
+  /* "Fortuna.pyx":950
  * 
  * def beta_variate(alpha: float, beta: float) -> float:
  *     return _beta(alpha, beta)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyFloat_FromDouble(Storm::GetFloat::beta_variate(__pyx_v_alpha, __pyx_v_beta)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 935, __pyx_L1_error)
+  __pyx_t_1 = PyFloat_FromDouble(Storm::GetFloat::beta_variate(__pyx_v_alpha, __pyx_v_beta)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 950, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "Fortuna.pyx":934
+  /* "Fortuna.pyx":949
  * 
  * 
  * def beta_variate(alpha: float, beta: float) -> float:             # <<<<<<<<<<<<<<
  *     return _beta(alpha, beta)
  * 
  */
 
@@ -24514,15 +25079,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "Fortuna.pyx":938
+/* "Fortuna.pyx":953
  * 
  * 
  * def pareto_variate(alpha: float) -> float:             # <<<<<<<<<<<<<<
  *     return _pareto(alpha)
  * 
  */
 
@@ -24576,31 +25141,31 @@
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_alpha)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 938, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 953, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "pareto_variate") < 0)) __PYX_ERR(0, 938, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "pareto_variate") < 0)) __PYX_ERR(0, 953, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs != 1)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
     }
-    __pyx_v_alpha = __pyx_PyFloat_AsDouble(values[0]); if (unlikely((__pyx_v_alpha == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 938, __pyx_L3_error)
+    __pyx_v_alpha = __pyx_PyFloat_AsDouble(values[0]); if (unlikely((__pyx_v_alpha == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 953, __pyx_L3_error)
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("pareto_variate", 1, 1, 1, __pyx_nargs); __PYX_ERR(0, 938, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("pareto_variate", 1, 1, 1, __pyx_nargs); __PYX_ERR(0, 953, __pyx_L3_error)
   __pyx_L6_skip:;
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
@@ -24628,29 +25193,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("pareto_variate", 1);
 
-  /* "Fortuna.pyx":939
+  /* "Fortuna.pyx":954
  * 
  * def pareto_variate(alpha: float) -> float:
  *     return _pareto(alpha)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyFloat_FromDouble(Storm::GetFloat::pareto_variate(__pyx_v_alpha)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 939, __pyx_L1_error)
+  __pyx_t_1 = PyFloat_FromDouble(Storm::GetFloat::pareto_variate(__pyx_v_alpha)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 954, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "Fortuna.pyx":938
+  /* "Fortuna.pyx":953
  * 
  * 
  * def pareto_variate(alpha: float) -> float:             # <<<<<<<<<<<<<<
  *     return _pareto(alpha)
  * 
  */
 
@@ -24661,15 +25226,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "Fortuna.pyx":942
+/* "Fortuna.pyx":957
  * 
  * 
  * def vonmises_variate(mu: float, kappa: float) -> float:             # <<<<<<<<<<<<<<
  *     return _vonmises(mu, kappa)
  * 
  */
 
@@ -24726,43 +25291,43 @@
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_mu)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 942, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 957, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_kappa)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[1]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 942, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 957, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("vonmises_variate", 1, 2, 2, 1); __PYX_ERR(0, 942, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("vonmises_variate", 1, 2, 2, 1); __PYX_ERR(0, 957, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "vonmises_variate") < 0)) __PYX_ERR(0, 942, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "vonmises_variate") < 0)) __PYX_ERR(0, 957, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs != 2)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
       values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
     }
-    __pyx_v_mu = __pyx_PyFloat_AsDouble(values[0]); if (unlikely((__pyx_v_mu == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 942, __pyx_L3_error)
-    __pyx_v_kappa = __pyx_PyFloat_AsDouble(values[1]); if (unlikely((__pyx_v_kappa == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 942, __pyx_L3_error)
+    __pyx_v_mu = __pyx_PyFloat_AsDouble(values[0]); if (unlikely((__pyx_v_mu == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 957, __pyx_L3_error)
+    __pyx_v_kappa = __pyx_PyFloat_AsDouble(values[1]); if (unlikely((__pyx_v_kappa == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 957, __pyx_L3_error)
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("vonmises_variate", 1, 2, 2, __pyx_nargs); __PYX_ERR(0, 942, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("vonmises_variate", 1, 2, 2, __pyx_nargs); __PYX_ERR(0, 957, __pyx_L3_error)
   __pyx_L6_skip:;
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
@@ -24790,29 +25355,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("vonmises_variate", 1);
 
-  /* "Fortuna.pyx":943
+  /* "Fortuna.pyx":958
  * 
  * def vonmises_variate(mu: float, kappa: float) -> float:
  *     return _vonmises(mu, kappa)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyFloat_FromDouble(Storm::GetFloat::vonmises_variate(__pyx_v_mu, __pyx_v_kappa)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 943, __pyx_L1_error)
+  __pyx_t_1 = PyFloat_FromDouble(Storm::GetFloat::vonmises_variate(__pyx_v_mu, __pyx_v_kappa)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 958, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "Fortuna.pyx":942
+  /* "Fortuna.pyx":957
  * 
  * 
  * def vonmises_variate(mu: float, kappa: float) -> float:             # <<<<<<<<<<<<<<
  *     return _vonmises(mu, kappa)
  * 
  */
 
@@ -24823,15 +25388,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "Fortuna.pyx":946
+/* "Fortuna.pyx":961
  * 
  * 
  * def bernoulli_variate(ratio_of_truth: float) -> bool:             # <<<<<<<<<<<<<<
  *     return _bernoulli(ratio_of_truth) == 1
  * 
  */
 
@@ -24885,31 +25450,31 @@
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_ratio_of_truth)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 946, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 961, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "bernoulli_variate") < 0)) __PYX_ERR(0, 946, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "bernoulli_variate") < 0)) __PYX_ERR(0, 961, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs != 1)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
     }
-    __pyx_v_ratio_of_truth = __pyx_PyFloat_AsDouble(values[0]); if (unlikely((__pyx_v_ratio_of_truth == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 946, __pyx_L3_error)
+    __pyx_v_ratio_of_truth = __pyx_PyFloat_AsDouble(values[0]); if (unlikely((__pyx_v_ratio_of_truth == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 961, __pyx_L3_error)
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("bernoulli_variate", 1, 1, 1, __pyx_nargs); __PYX_ERR(0, 946, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("bernoulli_variate", 1, 1, 1, __pyx_nargs); __PYX_ERR(0, 961, __pyx_L3_error)
   __pyx_L6_skip:;
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
@@ -24937,29 +25502,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("bernoulli_variate", 1);
 
-  /* "Fortuna.pyx":947
+  /* "Fortuna.pyx":962
  * 
  * def bernoulli_variate(ratio_of_truth: float) -> bool:
  *     return _bernoulli(ratio_of_truth) == 1             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyBool_FromLong((Storm::GetBool::bernoulli_variate(__pyx_v_ratio_of_truth) == 1)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 947, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyBool_FromLong((Storm::GetBool::bernoulli_variate(__pyx_v_ratio_of_truth) == 1)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 962, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "Fortuna.pyx":946
+  /* "Fortuna.pyx":961
  * 
  * 
  * def bernoulli_variate(ratio_of_truth: float) -> bool:             # <<<<<<<<<<<<<<
  *     return _bernoulli(ratio_of_truth) == 1
  * 
  */
 
@@ -24970,15 +25535,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "Fortuna.pyx":950
+/* "Fortuna.pyx":965
  * 
  * 
  * def binomial_variate(number_of_trials: int, probability: float) -> int:             # <<<<<<<<<<<<<<
  *     return _binomial(number_of_trials, probability)
  * 
  */
 
@@ -25035,57 +25600,57 @@
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_number_of_trials)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 950, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 965, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_probability)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[1]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 950, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 965, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("binomial_variate", 1, 2, 2, 1); __PYX_ERR(0, 950, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("binomial_variate", 1, 2, 2, 1); __PYX_ERR(0, 965, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "binomial_variate") < 0)) __PYX_ERR(0, 950, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "binomial_variate") < 0)) __PYX_ERR(0, 965, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs != 2)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
       values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
     }
     __pyx_v_number_of_trials = ((PyObject*)values[0]);
-    __pyx_v_probability = __pyx_PyFloat_AsDouble(values[1]); if (unlikely((__pyx_v_probability == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 950, __pyx_L3_error)
+    __pyx_v_probability = __pyx_PyFloat_AsDouble(values[1]); if (unlikely((__pyx_v_probability == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 965, __pyx_L3_error)
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("binomial_variate", 1, 2, 2, __pyx_nargs); __PYX_ERR(0, 950, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("binomial_variate", 1, 2, 2, __pyx_nargs); __PYX_ERR(0, 965, __pyx_L3_error)
   __pyx_L6_skip:;
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_AddTraceback("Fortuna.binomial_variate", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_number_of_trials), (&PyInt_Type), 0, "number_of_trials", 1))) __PYX_ERR(0, 950, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_number_of_trials), (&PyInt_Type), 0, "number_of_trials", 1))) __PYX_ERR(0, 965, __pyx_L1_error)
   __pyx_r = __pyx_pf_7Fortuna_104binomial_variate(__pyx_self, __pyx_v_number_of_trials, __pyx_v_probability);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
@@ -25105,31 +25670,31 @@
   PY_LONG_LONG __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("binomial_variate", 1);
 
-  /* "Fortuna.pyx":951
+  /* "Fortuna.pyx":966
  * 
  * def binomial_variate(number_of_trials: int, probability: float) -> int:
  *     return _binomial(number_of_trials, probability)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyInt_As_PY_LONG_LONG(__pyx_v_number_of_trials); if (unlikely((__pyx_t_1 == (PY_LONG_LONG)-1) && PyErr_Occurred())) __PYX_ERR(0, 951, __pyx_L1_error)
-  __pyx_t_2 = __Pyx_PyInt_From_PY_LONG_LONG(Storm::GetInt::binomial_variate(__pyx_t_1, __pyx_v_probability)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 951, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_As_PY_LONG_LONG(__pyx_v_number_of_trials); if (unlikely((__pyx_t_1 == (PY_LONG_LONG)-1) && PyErr_Occurred())) __PYX_ERR(0, 966, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_From_PY_LONG_LONG(Storm::GetInt::binomial_variate(__pyx_t_1, __pyx_v_probability)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 966, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (!(likely(__Pyx_Py3Int_CheckExact(__pyx_t_2)) || __Pyx_RaiseUnexpectedTypeError("int", __pyx_t_2))) __PYX_ERR(0, 951, __pyx_L1_error)
+  if (!(likely(__Pyx_Py3Int_CheckExact(__pyx_t_2)) || __Pyx_RaiseUnexpectedTypeError("int", __pyx_t_2))) __PYX_ERR(0, 966, __pyx_L1_error)
   __pyx_r = ((PyObject*)__pyx_t_2);
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "Fortuna.pyx":950
+  /* "Fortuna.pyx":965
  * 
  * 
  * def binomial_variate(number_of_trials: int, probability: float) -> int:             # <<<<<<<<<<<<<<
  *     return _binomial(number_of_trials, probability)
  * 
  */
 
@@ -25140,15 +25705,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "Fortuna.pyx":954
+/* "Fortuna.pyx":969
  * 
  * 
  * def negative_binomial_variate(number_of_trials: int, probability: float) -> int:             # <<<<<<<<<<<<<<
  *     return _neg_binomial(number_of_trials, probability)
  * 
  */
 
@@ -25205,57 +25770,57 @@
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_number_of_trials)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 954, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 969, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_probability)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[1]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 954, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 969, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("negative_binomial_variate", 1, 2, 2, 1); __PYX_ERR(0, 954, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("negative_binomial_variate", 1, 2, 2, 1); __PYX_ERR(0, 969, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "negative_binomial_variate") < 0)) __PYX_ERR(0, 954, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "negative_binomial_variate") < 0)) __PYX_ERR(0, 969, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs != 2)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
       values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
     }
     __pyx_v_number_of_trials = ((PyObject*)values[0]);
-    __pyx_v_probability = __pyx_PyFloat_AsDouble(values[1]); if (unlikely((__pyx_v_probability == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 954, __pyx_L3_error)
+    __pyx_v_probability = __pyx_PyFloat_AsDouble(values[1]); if (unlikely((__pyx_v_probability == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 969, __pyx_L3_error)
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("negative_binomial_variate", 1, 2, 2, __pyx_nargs); __PYX_ERR(0, 954, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("negative_binomial_variate", 1, 2, 2, __pyx_nargs); __PYX_ERR(0, 969, __pyx_L3_error)
   __pyx_L6_skip:;
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_AddTraceback("Fortuna.negative_binomial_variate", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_number_of_trials), (&PyInt_Type), 0, "number_of_trials", 1))) __PYX_ERR(0, 954, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_number_of_trials), (&PyInt_Type), 0, "number_of_trials", 1))) __PYX_ERR(0, 969, __pyx_L1_error)
   __pyx_r = __pyx_pf_7Fortuna_106negative_binomial_variate(__pyx_self, __pyx_v_number_of_trials, __pyx_v_probability);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
@@ -25275,31 +25840,31 @@
   PY_LONG_LONG __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("negative_binomial_variate", 1);
 
-  /* "Fortuna.pyx":955
+  /* "Fortuna.pyx":970
  * 
  * def negative_binomial_variate(number_of_trials: int, probability: float) -> int:
  *     return _neg_binomial(number_of_trials, probability)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyInt_As_PY_LONG_LONG(__pyx_v_number_of_trials); if (unlikely((__pyx_t_1 == (PY_LONG_LONG)-1) && PyErr_Occurred())) __PYX_ERR(0, 955, __pyx_L1_error)
-  __pyx_t_2 = __Pyx_PyInt_From_PY_LONG_LONG(Storm::GetInt::negative_binomial_variate(__pyx_t_1, __pyx_v_probability)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 955, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_As_PY_LONG_LONG(__pyx_v_number_of_trials); if (unlikely((__pyx_t_1 == (PY_LONG_LONG)-1) && PyErr_Occurred())) __PYX_ERR(0, 970, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_From_PY_LONG_LONG(Storm::GetInt::negative_binomial_variate(__pyx_t_1, __pyx_v_probability)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 970, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (!(likely(__Pyx_Py3Int_CheckExact(__pyx_t_2)) || __Pyx_RaiseUnexpectedTypeError("int", __pyx_t_2))) __PYX_ERR(0, 955, __pyx_L1_error)
+  if (!(likely(__Pyx_Py3Int_CheckExact(__pyx_t_2)) || __Pyx_RaiseUnexpectedTypeError("int", __pyx_t_2))) __PYX_ERR(0, 970, __pyx_L1_error)
   __pyx_r = ((PyObject*)__pyx_t_2);
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "Fortuna.pyx":954
+  /* "Fortuna.pyx":969
  * 
  * 
  * def negative_binomial_variate(number_of_trials: int, probability: float) -> int:             # <<<<<<<<<<<<<<
  *     return _neg_binomial(number_of_trials, probability)
  * 
  */
 
@@ -25310,15 +25875,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "Fortuna.pyx":958
+/* "Fortuna.pyx":973
  * 
  * 
  * def geometric_variate(probability: float) -> int:             # <<<<<<<<<<<<<<
  *     return _geometric(probability)
  * 
  */
 
@@ -25372,31 +25937,31 @@
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_probability)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 958, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 973, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "geometric_variate") < 0)) __PYX_ERR(0, 958, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "geometric_variate") < 0)) __PYX_ERR(0, 973, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs != 1)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
     }
-    __pyx_v_probability = __pyx_PyFloat_AsDouble(values[0]); if (unlikely((__pyx_v_probability == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 958, __pyx_L3_error)
+    __pyx_v_probability = __pyx_PyFloat_AsDouble(values[0]); if (unlikely((__pyx_v_probability == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 973, __pyx_L3_error)
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("geometric_variate", 1, 1, 1, __pyx_nargs); __PYX_ERR(0, 958, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("geometric_variate", 1, 1, 1, __pyx_nargs); __PYX_ERR(0, 973, __pyx_L3_error)
   __pyx_L6_skip:;
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
@@ -25424,30 +25989,30 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("geometric_variate", 1);
 
-  /* "Fortuna.pyx":959
+  /* "Fortuna.pyx":974
  * 
  * def geometric_variate(probability: float) -> int:
  *     return _geometric(probability)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyInt_From_PY_LONG_LONG(Storm::GetInt::geometric_variate(__pyx_v_probability)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 959, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_PY_LONG_LONG(Storm::GetInt::geometric_variate(__pyx_v_probability)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 974, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (!(likely(__Pyx_Py3Int_CheckExact(__pyx_t_1)) || __Pyx_RaiseUnexpectedTypeError("int", __pyx_t_1))) __PYX_ERR(0, 959, __pyx_L1_error)
+  if (!(likely(__Pyx_Py3Int_CheckExact(__pyx_t_1)) || __Pyx_RaiseUnexpectedTypeError("int", __pyx_t_1))) __PYX_ERR(0, 974, __pyx_L1_error)
   __pyx_r = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "Fortuna.pyx":958
+  /* "Fortuna.pyx":973
  * 
  * 
  * def geometric_variate(probability: float) -> int:             # <<<<<<<<<<<<<<
  *     return _geometric(probability)
  * 
  */
 
@@ -25458,15 +26023,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "Fortuna.pyx":962
+/* "Fortuna.pyx":977
  * 
  * 
  * def poisson_variate(mean: float) -> int:             # <<<<<<<<<<<<<<
  *     return _poisson(mean)
  * 
  */
 
@@ -25520,31 +26085,31 @@
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_mean)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 962, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 977, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "poisson_variate") < 0)) __PYX_ERR(0, 962, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "poisson_variate") < 0)) __PYX_ERR(0, 977, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs != 1)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
     }
-    __pyx_v_mean = __pyx_PyFloat_AsDouble(values[0]); if (unlikely((__pyx_v_mean == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 962, __pyx_L3_error)
+    __pyx_v_mean = __pyx_PyFloat_AsDouble(values[0]); if (unlikely((__pyx_v_mean == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 977, __pyx_L3_error)
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("poisson_variate", 1, 1, 1, __pyx_nargs); __PYX_ERR(0, 962, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("poisson_variate", 1, 1, 1, __pyx_nargs); __PYX_ERR(0, 977, __pyx_L3_error)
   __pyx_L6_skip:;
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
@@ -25572,30 +26137,30 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("poisson_variate", 1);
 
-  /* "Fortuna.pyx":963
+  /* "Fortuna.pyx":978
  * 
  * def poisson_variate(mean: float) -> int:
  *     return _poisson(mean)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyInt_From_PY_LONG_LONG(Storm::GetInt::poisson_variate(__pyx_v_mean)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 963, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_PY_LONG_LONG(Storm::GetInt::poisson_variate(__pyx_v_mean)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 978, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (!(likely(__Pyx_Py3Int_CheckExact(__pyx_t_1)) || __Pyx_RaiseUnexpectedTypeError("int", __pyx_t_1))) __PYX_ERR(0, 963, __pyx_L1_error)
+  if (!(likely(__Pyx_Py3Int_CheckExact(__pyx_t_1)) || __Pyx_RaiseUnexpectedTypeError("int", __pyx_t_1))) __PYX_ERR(0, 978, __pyx_L1_error)
   __pyx_r = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "Fortuna.pyx":962
+  /* "Fortuna.pyx":977
  * 
  * 
  * def poisson_variate(mean: float) -> int:             # <<<<<<<<<<<<<<
  *     return _poisson(mean)
  * 
  */
 
@@ -25606,15 +26171,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "Fortuna.pyx":966
+/* "Fortuna.pyx":981
  * 
  * 
  * def exponential_variate(lambda_rate: float) -> float:             # <<<<<<<<<<<<<<
  *     return _exponential(lambda_rate)
  * 
  */
 
@@ -25668,31 +26233,31 @@
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_lambda_rate)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 966, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 981, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "exponential_variate") < 0)) __PYX_ERR(0, 966, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "exponential_variate") < 0)) __PYX_ERR(0, 981, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs != 1)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
     }
-    __pyx_v_lambda_rate = __pyx_PyFloat_AsDouble(values[0]); if (unlikely((__pyx_v_lambda_rate == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 966, __pyx_L3_error)
+    __pyx_v_lambda_rate = __pyx_PyFloat_AsDouble(values[0]); if (unlikely((__pyx_v_lambda_rate == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 981, __pyx_L3_error)
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("exponential_variate", 1, 1, 1, __pyx_nargs); __PYX_ERR(0, 966, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("exponential_variate", 1, 1, 1, __pyx_nargs); __PYX_ERR(0, 981, __pyx_L3_error)
   __pyx_L6_skip:;
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
@@ -25720,29 +26285,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("exponential_variate", 1);
 
-  /* "Fortuna.pyx":967
+  /* "Fortuna.pyx":982
  * 
  * def exponential_variate(lambda_rate: float) -> float:
  *     return _exponential(lambda_rate)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyFloat_FromDouble(Storm::GetFloat::exponential_variate(__pyx_v_lambda_rate)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 967, __pyx_L1_error)
+  __pyx_t_1 = PyFloat_FromDouble(Storm::GetFloat::exponential_variate(__pyx_v_lambda_rate)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 982, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "Fortuna.pyx":966
+  /* "Fortuna.pyx":981
  * 
  * 
  * def exponential_variate(lambda_rate: float) -> float:             # <<<<<<<<<<<<<<
  *     return _exponential(lambda_rate)
  * 
  */
 
@@ -25753,15 +26318,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "Fortuna.pyx":970
+/* "Fortuna.pyx":985
  * 
  * 
  * def gamma_variate(shape: float, scale: float) -> float:             # <<<<<<<<<<<<<<
  *     return _gamma(shape, scale)
  * 
  */
 
@@ -25818,43 +26383,43 @@
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_shape)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 970, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 985, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_scale)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[1]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 970, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 985, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("gamma_variate", 1, 2, 2, 1); __PYX_ERR(0, 970, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("gamma_variate", 1, 2, 2, 1); __PYX_ERR(0, 985, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "gamma_variate") < 0)) __PYX_ERR(0, 970, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "gamma_variate") < 0)) __PYX_ERR(0, 985, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs != 2)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
       values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
     }
-    __pyx_v_shape = __pyx_PyFloat_AsDouble(values[0]); if (unlikely((__pyx_v_shape == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 970, __pyx_L3_error)
-    __pyx_v_scale = __pyx_PyFloat_AsDouble(values[1]); if (unlikely((__pyx_v_scale == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 970, __pyx_L3_error)
+    __pyx_v_shape = __pyx_PyFloat_AsDouble(values[0]); if (unlikely((__pyx_v_shape == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 985, __pyx_L3_error)
+    __pyx_v_scale = __pyx_PyFloat_AsDouble(values[1]); if (unlikely((__pyx_v_scale == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 985, __pyx_L3_error)
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("gamma_variate", 1, 2, 2, __pyx_nargs); __PYX_ERR(0, 970, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("gamma_variate", 1, 2, 2, __pyx_nargs); __PYX_ERR(0, 985, __pyx_L3_error)
   __pyx_L6_skip:;
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
@@ -25882,29 +26447,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("gamma_variate", 1);
 
-  /* "Fortuna.pyx":971
+  /* "Fortuna.pyx":986
  * 
  * def gamma_variate(shape: float, scale: float) -> float:
  *     return _gamma(shape, scale)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyFloat_FromDouble(Storm::GetFloat::gamma_variate(__pyx_v_shape, __pyx_v_scale)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 971, __pyx_L1_error)
+  __pyx_t_1 = PyFloat_FromDouble(Storm::GetFloat::gamma_variate(__pyx_v_shape, __pyx_v_scale)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 986, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "Fortuna.pyx":970
+  /* "Fortuna.pyx":985
  * 
  * 
  * def gamma_variate(shape: float, scale: float) -> float:             # <<<<<<<<<<<<<<
  *     return _gamma(shape, scale)
  * 
  */
 
@@ -25915,15 +26480,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "Fortuna.pyx":974
+/* "Fortuna.pyx":989
  * 
  * 
  * def weibull_variate(shape: float, scale: float) -> float:             # <<<<<<<<<<<<<<
  *     return _weibull(shape, scale)
  * 
  */
 
@@ -25980,43 +26545,43 @@
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_shape)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 974, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 989, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_scale)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[1]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 974, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 989, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("weibull_variate", 1, 2, 2, 1); __PYX_ERR(0, 974, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("weibull_variate", 1, 2, 2, 1); __PYX_ERR(0, 989, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "weibull_variate") < 0)) __PYX_ERR(0, 974, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "weibull_variate") < 0)) __PYX_ERR(0, 989, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs != 2)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
       values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
     }
-    __pyx_v_shape = __pyx_PyFloat_AsDouble(values[0]); if (unlikely((__pyx_v_shape == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 974, __pyx_L3_error)
-    __pyx_v_scale = __pyx_PyFloat_AsDouble(values[1]); if (unlikely((__pyx_v_scale == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 974, __pyx_L3_error)
+    __pyx_v_shape = __pyx_PyFloat_AsDouble(values[0]); if (unlikely((__pyx_v_shape == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 989, __pyx_L3_error)
+    __pyx_v_scale = __pyx_PyFloat_AsDouble(values[1]); if (unlikely((__pyx_v_scale == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 989, __pyx_L3_error)
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("weibull_variate", 1, 2, 2, __pyx_nargs); __PYX_ERR(0, 974, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("weibull_variate", 1, 2, 2, __pyx_nargs); __PYX_ERR(0, 989, __pyx_L3_error)
   __pyx_L6_skip:;
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
@@ -26044,29 +26609,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("weibull_variate", 1);
 
-  /* "Fortuna.pyx":975
+  /* "Fortuna.pyx":990
  * 
  * def weibull_variate(shape: float, scale: float) -> float:
  *     return _weibull(shape, scale)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyFloat_FromDouble(Storm::GetFloat::weibull_variate(__pyx_v_shape, __pyx_v_scale)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 975, __pyx_L1_error)
+  __pyx_t_1 = PyFloat_FromDouble(Storm::GetFloat::weibull_variate(__pyx_v_shape, __pyx_v_scale)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 990, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "Fortuna.pyx":974
+  /* "Fortuna.pyx":989
  * 
  * 
  * def weibull_variate(shape: float, scale: float) -> float:             # <<<<<<<<<<<<<<
  *     return _weibull(shape, scale)
  * 
  */
 
@@ -26077,15 +26642,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "Fortuna.pyx":978
+/* "Fortuna.pyx":993
  * 
  * 
  * def normal_variate(mean: float, std_dev: float) -> float:             # <<<<<<<<<<<<<<
  *     return _normal(mean, std_dev)
  * 
  */
 
@@ -26142,43 +26707,43 @@
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_mean)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 978, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 993, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_std_dev)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[1]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 978, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 993, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("normal_variate", 1, 2, 2, 1); __PYX_ERR(0, 978, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("normal_variate", 1, 2, 2, 1); __PYX_ERR(0, 993, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "normal_variate") < 0)) __PYX_ERR(0, 978, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "normal_variate") < 0)) __PYX_ERR(0, 993, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs != 2)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
       values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
     }
-    __pyx_v_mean = __pyx_PyFloat_AsDouble(values[0]); if (unlikely((__pyx_v_mean == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 978, __pyx_L3_error)
-    __pyx_v_std_dev = __pyx_PyFloat_AsDouble(values[1]); if (unlikely((__pyx_v_std_dev == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 978, __pyx_L3_error)
+    __pyx_v_mean = __pyx_PyFloat_AsDouble(values[0]); if (unlikely((__pyx_v_mean == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 993, __pyx_L3_error)
+    __pyx_v_std_dev = __pyx_PyFloat_AsDouble(values[1]); if (unlikely((__pyx_v_std_dev == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 993, __pyx_L3_error)
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("normal_variate", 1, 2, 2, __pyx_nargs); __PYX_ERR(0, 978, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("normal_variate", 1, 2, 2, __pyx_nargs); __PYX_ERR(0, 993, __pyx_L3_error)
   __pyx_L6_skip:;
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
@@ -26206,29 +26771,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("normal_variate", 1);
 
-  /* "Fortuna.pyx":979
+  /* "Fortuna.pyx":994
  * 
  * def normal_variate(mean: float, std_dev: float) -> float:
  *     return _normal(mean, std_dev)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyFloat_FromDouble(Storm::GetFloat::normal_variate(__pyx_v_mean, __pyx_v_std_dev)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 979, __pyx_L1_error)
+  __pyx_t_1 = PyFloat_FromDouble(Storm::GetFloat::normal_variate(__pyx_v_mean, __pyx_v_std_dev)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 994, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "Fortuna.pyx":978
+  /* "Fortuna.pyx":993
  * 
  * 
  * def normal_variate(mean: float, std_dev: float) -> float:             # <<<<<<<<<<<<<<
  *     return _normal(mean, std_dev)
  * 
  */
 
@@ -26239,15 +26804,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "Fortuna.pyx":982
+/* "Fortuna.pyx":997
  * 
  * 
  * def log_normal_variate(log_mean: float, log_deviation: float) -> float:             # <<<<<<<<<<<<<<
  *     return _log_normal(log_mean, log_deviation)
  * 
  */
 
@@ -26304,43 +26869,43 @@
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_log_mean)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 982, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 997, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_log_deviation)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[1]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 982, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 997, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("log_normal_variate", 1, 2, 2, 1); __PYX_ERR(0, 982, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("log_normal_variate", 1, 2, 2, 1); __PYX_ERR(0, 997, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "log_normal_variate") < 0)) __PYX_ERR(0, 982, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "log_normal_variate") < 0)) __PYX_ERR(0, 997, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs != 2)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
       values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
     }
-    __pyx_v_log_mean = __pyx_PyFloat_AsDouble(values[0]); if (unlikely((__pyx_v_log_mean == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 982, __pyx_L3_error)
-    __pyx_v_log_deviation = __pyx_PyFloat_AsDouble(values[1]); if (unlikely((__pyx_v_log_deviation == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 982, __pyx_L3_error)
+    __pyx_v_log_mean = __pyx_PyFloat_AsDouble(values[0]); if (unlikely((__pyx_v_log_mean == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 997, __pyx_L3_error)
+    __pyx_v_log_deviation = __pyx_PyFloat_AsDouble(values[1]); if (unlikely((__pyx_v_log_deviation == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 997, __pyx_L3_error)
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("log_normal_variate", 1, 2, 2, __pyx_nargs); __PYX_ERR(0, 982, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("log_normal_variate", 1, 2, 2, __pyx_nargs); __PYX_ERR(0, 997, __pyx_L3_error)
   __pyx_L6_skip:;
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
@@ -26368,29 +26933,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("log_normal_variate", 1);
 
-  /* "Fortuna.pyx":983
+  /* "Fortuna.pyx":998
  * 
  * def log_normal_variate(log_mean: float, log_deviation: float) -> float:
  *     return _log_normal(log_mean, log_deviation)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyFloat_FromDouble(Storm::GetFloat::log_normal_variate(__pyx_v_log_mean, __pyx_v_log_deviation)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 983, __pyx_L1_error)
+  __pyx_t_1 = PyFloat_FromDouble(Storm::GetFloat::log_normal_variate(__pyx_v_log_mean, __pyx_v_log_deviation)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 998, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "Fortuna.pyx":982
+  /* "Fortuna.pyx":997
  * 
  * 
  * def log_normal_variate(log_mean: float, log_deviation: float) -> float:             # <<<<<<<<<<<<<<
  *     return _log_normal(log_mean, log_deviation)
  * 
  */
 
@@ -26401,15 +26966,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "Fortuna.pyx":986
+/* "Fortuna.pyx":1001
  * 
  * 
  * def extreme_value_variate(location: float, scale: float) -> float:             # <<<<<<<<<<<<<<
  *     return _extreme_value(location, scale)
  * 
  */
 
@@ -26466,43 +27031,43 @@
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_location)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 986, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 1001, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_scale)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[1]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 986, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 1001, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("extreme_value_variate", 1, 2, 2, 1); __PYX_ERR(0, 986, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("extreme_value_variate", 1, 2, 2, 1); __PYX_ERR(0, 1001, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "extreme_value_variate") < 0)) __PYX_ERR(0, 986, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "extreme_value_variate") < 0)) __PYX_ERR(0, 1001, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs != 2)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
       values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
     }
-    __pyx_v_location = __pyx_PyFloat_AsDouble(values[0]); if (unlikely((__pyx_v_location == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 986, __pyx_L3_error)
-    __pyx_v_scale = __pyx_PyFloat_AsDouble(values[1]); if (unlikely((__pyx_v_scale == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 986, __pyx_L3_error)
+    __pyx_v_location = __pyx_PyFloat_AsDouble(values[0]); if (unlikely((__pyx_v_location == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 1001, __pyx_L3_error)
+    __pyx_v_scale = __pyx_PyFloat_AsDouble(values[1]); if (unlikely((__pyx_v_scale == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 1001, __pyx_L3_error)
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("extreme_value_variate", 1, 2, 2, __pyx_nargs); __PYX_ERR(0, 986, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("extreme_value_variate", 1, 2, 2, __pyx_nargs); __PYX_ERR(0, 1001, __pyx_L3_error)
   __pyx_L6_skip:;
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
@@ -26530,29 +27095,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("extreme_value_variate", 1);
 
-  /* "Fortuna.pyx":987
+  /* "Fortuna.pyx":1002
  * 
  * def extreme_value_variate(location: float, scale: float) -> float:
  *     return _extreme_value(location, scale)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyFloat_FromDouble(Storm::GetFloat::extreme_value_variate(__pyx_v_location, __pyx_v_scale)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 987, __pyx_L1_error)
+  __pyx_t_1 = PyFloat_FromDouble(Storm::GetFloat::extreme_value_variate(__pyx_v_location, __pyx_v_scale)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1002, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "Fortuna.pyx":986
+  /* "Fortuna.pyx":1001
  * 
  * 
  * def extreme_value_variate(location: float, scale: float) -> float:             # <<<<<<<<<<<<<<
  *     return _extreme_value(location, scale)
  * 
  */
 
@@ -26563,15 +27128,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "Fortuna.pyx":990
+/* "Fortuna.pyx":1005
  * 
  * 
  * def chi_squared_variate(degrees_of_freedom: float) -> float:             # <<<<<<<<<<<<<<
  *     return _chi_squared(degrees_of_freedom)
  * 
  */
 
@@ -26625,31 +27190,31 @@
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_degrees_of_freedom)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 990, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 1005, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "chi_squared_variate") < 0)) __PYX_ERR(0, 990, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "chi_squared_variate") < 0)) __PYX_ERR(0, 1005, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs != 1)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
     }
-    __pyx_v_degrees_of_freedom = __pyx_PyFloat_AsDouble(values[0]); if (unlikely((__pyx_v_degrees_of_freedom == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 990, __pyx_L3_error)
+    __pyx_v_degrees_of_freedom = __pyx_PyFloat_AsDouble(values[0]); if (unlikely((__pyx_v_degrees_of_freedom == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 1005, __pyx_L3_error)
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("chi_squared_variate", 1, 1, 1, __pyx_nargs); __PYX_ERR(0, 990, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("chi_squared_variate", 1, 1, 1, __pyx_nargs); __PYX_ERR(0, 1005, __pyx_L3_error)
   __pyx_L6_skip:;
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
@@ -26677,29 +27242,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("chi_squared_variate", 1);
 
-  /* "Fortuna.pyx":991
+  /* "Fortuna.pyx":1006
  * 
  * def chi_squared_variate(degrees_of_freedom: float) -> float:
  *     return _chi_squared(degrees_of_freedom)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyFloat_FromDouble(Storm::GetFloat::chi_squared_variate(__pyx_v_degrees_of_freedom)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 991, __pyx_L1_error)
+  __pyx_t_1 = PyFloat_FromDouble(Storm::GetFloat::chi_squared_variate(__pyx_v_degrees_of_freedom)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1006, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "Fortuna.pyx":990
+  /* "Fortuna.pyx":1005
  * 
  * 
  * def chi_squared_variate(degrees_of_freedom: float) -> float:             # <<<<<<<<<<<<<<
  *     return _chi_squared(degrees_of_freedom)
  * 
  */
 
@@ -26710,15 +27275,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "Fortuna.pyx":994
+/* "Fortuna.pyx":1009
  * 
  * 
  * def cauchy_variate(location: float, scale: float) -> float:             # <<<<<<<<<<<<<<
  *     return _cauchy(location, scale)
  * 
  */
 
@@ -26775,43 +27340,43 @@
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_location)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 994, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 1009, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_scale)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[1]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 994, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 1009, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("cauchy_variate", 1, 2, 2, 1); __PYX_ERR(0, 994, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("cauchy_variate", 1, 2, 2, 1); __PYX_ERR(0, 1009, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "cauchy_variate") < 0)) __PYX_ERR(0, 994, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "cauchy_variate") < 0)) __PYX_ERR(0, 1009, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs != 2)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
       values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
     }
-    __pyx_v_location = __pyx_PyFloat_AsDouble(values[0]); if (unlikely((__pyx_v_location == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 994, __pyx_L3_error)
-    __pyx_v_scale = __pyx_PyFloat_AsDouble(values[1]); if (unlikely((__pyx_v_scale == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 994, __pyx_L3_error)
+    __pyx_v_location = __pyx_PyFloat_AsDouble(values[0]); if (unlikely((__pyx_v_location == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 1009, __pyx_L3_error)
+    __pyx_v_scale = __pyx_PyFloat_AsDouble(values[1]); if (unlikely((__pyx_v_scale == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 1009, __pyx_L3_error)
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("cauchy_variate", 1, 2, 2, __pyx_nargs); __PYX_ERR(0, 994, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("cauchy_variate", 1, 2, 2, __pyx_nargs); __PYX_ERR(0, 1009, __pyx_L3_error)
   __pyx_L6_skip:;
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
@@ -26839,29 +27404,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("cauchy_variate", 1);
 
-  /* "Fortuna.pyx":995
+  /* "Fortuna.pyx":1010
  * 
  * def cauchy_variate(location: float, scale: float) -> float:
  *     return _cauchy(location, scale)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyFloat_FromDouble(Storm::GetFloat::cauchy_variate(__pyx_v_location, __pyx_v_scale)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 995, __pyx_L1_error)
+  __pyx_t_1 = PyFloat_FromDouble(Storm::GetFloat::cauchy_variate(__pyx_v_location, __pyx_v_scale)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1010, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "Fortuna.pyx":994
+  /* "Fortuna.pyx":1009
  * 
  * 
  * def cauchy_variate(location: float, scale: float) -> float:             # <<<<<<<<<<<<<<
  *     return _cauchy(location, scale)
  * 
  */
 
@@ -26872,15 +27437,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "Fortuna.pyx":998
+/* "Fortuna.pyx":1013
  * 
  * 
  * def fisher_f_variate(degrees_of_freedom_1: float, degrees_of_freedom_2: float) -> float:             # <<<<<<<<<<<<<<
  *     return _fisher_f(degrees_of_freedom_1, degrees_of_freedom_2)
  * 
  */
 
@@ -26937,43 +27502,43 @@
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_degrees_of_freedom_1)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 998, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 1013, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_degrees_of_freedom_2)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[1]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 998, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 1013, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("fisher_f_variate", 1, 2, 2, 1); __PYX_ERR(0, 998, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("fisher_f_variate", 1, 2, 2, 1); __PYX_ERR(0, 1013, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "fisher_f_variate") < 0)) __PYX_ERR(0, 998, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "fisher_f_variate") < 0)) __PYX_ERR(0, 1013, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs != 2)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
       values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
     }
-    __pyx_v_degrees_of_freedom_1 = __pyx_PyFloat_AsDouble(values[0]); if (unlikely((__pyx_v_degrees_of_freedom_1 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 998, __pyx_L3_error)
-    __pyx_v_degrees_of_freedom_2 = __pyx_PyFloat_AsDouble(values[1]); if (unlikely((__pyx_v_degrees_of_freedom_2 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 998, __pyx_L3_error)
+    __pyx_v_degrees_of_freedom_1 = __pyx_PyFloat_AsDouble(values[0]); if (unlikely((__pyx_v_degrees_of_freedom_1 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 1013, __pyx_L3_error)
+    __pyx_v_degrees_of_freedom_2 = __pyx_PyFloat_AsDouble(values[1]); if (unlikely((__pyx_v_degrees_of_freedom_2 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 1013, __pyx_L3_error)
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("fisher_f_variate", 1, 2, 2, __pyx_nargs); __PYX_ERR(0, 998, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("fisher_f_variate", 1, 2, 2, __pyx_nargs); __PYX_ERR(0, 1013, __pyx_L3_error)
   __pyx_L6_skip:;
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
@@ -27001,29 +27566,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("fisher_f_variate", 1);
 
-  /* "Fortuna.pyx":999
+  /* "Fortuna.pyx":1014
  * 
  * def fisher_f_variate(degrees_of_freedom_1: float, degrees_of_freedom_2: float) -> float:
  *     return _fisher_f(degrees_of_freedom_1, degrees_of_freedom_2)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyFloat_FromDouble(Storm::GetFloat::fisher_f_variate(__pyx_v_degrees_of_freedom_1, __pyx_v_degrees_of_freedom_2)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 999, __pyx_L1_error)
+  __pyx_t_1 = PyFloat_FromDouble(Storm::GetFloat::fisher_f_variate(__pyx_v_degrees_of_freedom_1, __pyx_v_degrees_of_freedom_2)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1014, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "Fortuna.pyx":998
+  /* "Fortuna.pyx":1013
  * 
  * 
  * def fisher_f_variate(degrees_of_freedom_1: float, degrees_of_freedom_2: float) -> float:             # <<<<<<<<<<<<<<
  *     return _fisher_f(degrees_of_freedom_1, degrees_of_freedom_2)
  * 
  */
 
@@ -27034,15 +27599,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "Fortuna.pyx":1002
+/* "Fortuna.pyx":1017
  * 
  * 
  * def student_t_variate(degrees_of_freedom: float) -> float:             # <<<<<<<<<<<<<<
  *     return _student_t(degrees_of_freedom)
  */
 
 /* Python wrapper */
@@ -27095,31 +27660,31 @@
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_degrees_of_freedom)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 1002, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 1017, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "student_t_variate") < 0)) __PYX_ERR(0, 1002, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "student_t_variate") < 0)) __PYX_ERR(0, 1017, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs != 1)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
     }
-    __pyx_v_degrees_of_freedom = __pyx_PyFloat_AsDouble(values[0]); if (unlikely((__pyx_v_degrees_of_freedom == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 1002, __pyx_L3_error)
+    __pyx_v_degrees_of_freedom = __pyx_PyFloat_AsDouble(values[0]); if (unlikely((__pyx_v_degrees_of_freedom == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 1017, __pyx_L3_error)
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("student_t_variate", 1, 1, 1, __pyx_nargs); __PYX_ERR(0, 1002, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("student_t_variate", 1, 1, 1, __pyx_nargs); __PYX_ERR(0, 1017, __pyx_L3_error)
   __pyx_L6_skip:;
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
@@ -27147,27 +27712,27 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("student_t_variate", 1);
 
-  /* "Fortuna.pyx":1003
+  /* "Fortuna.pyx":1018
  * 
  * def student_t_variate(degrees_of_freedom: float) -> float:
  *     return _student_t(degrees_of_freedom)             # <<<<<<<<<<<<<<
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyFloat_FromDouble(Storm::GetFloat::student_t_variate(__pyx_v_degrees_of_freedom)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1003, __pyx_L1_error)
+  __pyx_t_1 = PyFloat_FromDouble(Storm::GetFloat::student_t_variate(__pyx_v_degrees_of_freedom)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1018, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "Fortuna.pyx":1002
+  /* "Fortuna.pyx":1017
  * 
  * 
  * def student_t_variate(degrees_of_freedom: float) -> float:             # <<<<<<<<<<<<<<
  *     return _student_t(degrees_of_freedom)
  */
 
   /* function exit code */
@@ -27905,18 +28470,19 @@
     {&__pyx_n_s_FlexCat___init, __pyx_k_FlexCat___init, sizeof(__pyx_k_FlexCat___init), 0, 0, 1, 1},
     {&__pyx_kp_s_Flex_Cat_FlexCat_is_a_lot_like, __pyx_k_Flex_Cat_FlexCat_is_a_lot_like, sizeof(__pyx_k_Flex_Cat_FlexCat_is_a_lot_like), 0, 0, 1, 0},
     {&__pyx_n_s_Fortuna, __pyx_k_Fortuna, sizeof(__pyx_k_Fortuna), 0, 0, 1, 1},
     {&__pyx_kp_s_Fortuna_pyx, __pyx_k_Fortuna_pyx, sizeof(__pyx_k_Fortuna_pyx), 0, 0, 1, 0},
     {&__pyx_kp_u_Input_Error_Empty_Container, __pyx_k_Input_Error_Empty_Container, sizeof(__pyx_k_Input_Error_Empty_Container), 0, 1, 0, 0},
     {&__pyx_n_s_Iterable, __pyx_k_Iterable, sizeof(__pyx_k_Iterable), 0, 0, 1, 1},
     {&__pyx_kp_s_Iterable_str, __pyx_k_Iterable_str, sizeof(__pyx_k_Iterable_str), 0, 0, 1, 0},
+    {&__pyx_n_s_Iterator, __pyx_k_Iterator, sizeof(__pyx_k_Iterator), 0, 0, 1, 1},
     {&__pyx_n_s_MultiChoice, __pyx_k_MultiChoice, sizeof(__pyx_k_MultiChoice), 0, 0, 1, 1},
     {&__pyx_n_s_MultiChoice___call, __pyx_k_MultiChoice___call, sizeof(__pyx_k_MultiChoice___call), 0, 0, 1, 1},
     {&__pyx_n_s_MultiChoice___init, __pyx_k_MultiChoice___init, sizeof(__pyx_k_MultiChoice___init), 0, 0, 1, 1},
-    {&__pyx_kp_u_MultiChoice___init___line_881, __pyx_k_MultiChoice___init___line_881, sizeof(__pyx_k_MultiChoice___init___line_881), 0, 1, 0, 0},
+    {&__pyx_kp_u_MultiChoice___init___line_896, __pyx_k_MultiChoice___init___line_896, sizeof(__pyx_k_MultiChoice___init___line_896), 0, 1, 0, 0},
     {&__pyx_n_s_MultiChoice___init___locals_gene, __pyx_k_MultiChoice___init___locals_gene, sizeof(__pyx_k_MultiChoice___init___locals_gene), 0, 0, 1, 1},
     {&__pyx_n_s_MultiChoice__get_answer, __pyx_k_MultiChoice__get_answer, sizeof(__pyx_k_MultiChoice__get_answer), 0, 0, 1, 1},
     {&__pyx_kp_s_Multiple_Choice_MultiChoice_gen, __pyx_k_Multiple_Choice_MultiChoice_gen, sizeof(__pyx_k_Multiple_Choice_MultiChoice_gen), 0, 0, 1, 0},
     {&__pyx_kp_u_Multiple_Choice_param_query_Str, __pyx_k_Multiple_Choice_param_query_Str, sizeof(__pyx_k_Multiple_Choice_param_query_Str), 0, 1, 0, 0},
     {&__pyx_n_s_None, __pyx_k_None, sizeof(__pyx_k_None), 0, 0, 1, 1},
     {&__pyx_n_s_QuantumMonty, __pyx_k_QuantumMonty, sizeof(__pyx_k_QuantumMonty), 0, 0, 1, 1},
     {&__pyx_n_s_QuantumMonty___call, __pyx_k_QuantumMonty___call, sizeof(__pyx_k_QuantumMonty___call), 0, 0, 1, 1},
@@ -27945,23 +28511,26 @@
     {&__pyx_n_s_RelativeWeightedChoice, __pyx_k_RelativeWeightedChoice, sizeof(__pyx_k_RelativeWeightedChoice), 0, 0, 1, 1},
     {&__pyx_n_s_RelativeWeightedChoice___init, __pyx_k_RelativeWeightedChoice___init, sizeof(__pyx_k_RelativeWeightedChoice___init), 0, 0, 1, 1},
     {&__pyx_n_s_RelativeWeightedChoice___init_2, __pyx_k_RelativeWeightedChoice___init_2, sizeof(__pyx_k_RelativeWeightedChoice___init_2), 0, 0, 1, 1},
     {&__pyx_n_s_RelativeWeightedChoice___init_3, __pyx_k_RelativeWeightedChoice___init_3, sizeof(__pyx_k_RelativeWeightedChoice___init_3), 0, 0, 1, 1},
     {&__pyx_kp_s_Relative_Weighted_Choice, __pyx_k_Relative_Weighted_Choice, sizeof(__pyx_k_Relative_Weighted_Choice), 0, 0, 1, 0},
     {&__pyx_kp_u_Sample_size_k_is_larger_than_pop, __pyx_k_Sample_size_k_is_larger_than_pop, sizeof(__pyx_k_Sample_size_k_is_larger_than_pop), 0, 1, 0, 0},
     {&__pyx_n_s_TruffleShuffle, __pyx_k_TruffleShuffle, sizeof(__pyx_k_TruffleShuffle), 0, 0, 1, 1},
+    {&__pyx_n_s_TruffleShuffle2, __pyx_k_TruffleShuffle2, sizeof(__pyx_k_TruffleShuffle2), 0, 0, 1, 1},
+    {&__pyx_n_s_TruffleShuffle2___call, __pyx_k_TruffleShuffle2___call, sizeof(__pyx_k_TruffleShuffle2___call), 0, 0, 1, 1},
+    {&__pyx_n_s_TruffleShuffle2___init, __pyx_k_TruffleShuffle2___init, sizeof(__pyx_k_TruffleShuffle2___init), 0, 0, 1, 1},
     {&__pyx_n_s_TruffleShuffle___call, __pyx_k_TruffleShuffle___call, sizeof(__pyx_k_TruffleShuffle___call), 0, 0, 1, 1},
     {&__pyx_n_s_TruffleShuffle___init, __pyx_k_TruffleShuffle___init, sizeof(__pyx_k_TruffleShuffle___init), 0, 0, 1, 1},
     {&__pyx_kp_s_Truffle_Shuffle_Produces_random, __pyx_k_Truffle_Shuffle_Produces_random, sizeof(__pyx_k_Truffle_Shuffle_Produces_random), 0, 0, 1, 0},
     {&__pyx_n_s_TypeError, __pyx_k_TypeError, sizeof(__pyx_k_TypeError), 0, 0, 1, 1},
     {&__pyx_n_s_WeightedChoice, __pyx_k_WeightedChoice, sizeof(__pyx_k_WeightedChoice), 0, 0, 1, 1},
     {&__pyx_n_s_WeightedChoice___call, __pyx_k_WeightedChoice___call, sizeof(__pyx_k_WeightedChoice___call), 0, 0, 1, 1},
     {&__pyx_kp_s_Weighted_Choice_Base_Class_inte, __pyx_k_Weighted_Choice_Base_Class_inte, sizeof(__pyx_k_Weighted_Choice_Base_Class_inte), 0, 0, 1, 0},
     {&__pyx_n_s_ZeroCool, __pyx_k_ZeroCool, sizeof(__pyx_k_ZeroCool), 0, 0, 1, 1},
-    {&__pyx_n_s__162, __pyx_k__162, sizeof(__pyx_k__162), 0, 0, 1, 1},
+    {&__pyx_n_s__165, __pyx_k__165, sizeof(__pyx_k__165), 0, 0, 1, 1},
     {&__pyx_kp_u__2, __pyx_k__2, sizeof(__pyx_k__2), 0, 1, 0, 0},
     {&__pyx_kp_u__3, __pyx_k__3, sizeof(__pyx_k__3), 0, 1, 0, 0},
     {&__pyx_kp_u__4, __pyx_k__4, sizeof(__pyx_k__4), 0, 1, 0, 0},
     {&__pyx_kp_u__5, __pyx_k__5, sizeof(__pyx_k__5), 0, 1, 0, 0},
     {&__pyx_kp_u__6, __pyx_k__6, sizeof(__pyx_k__6), 0, 1, 0, 0},
     {&__pyx_kp_u__7, __pyx_k__7, sizeof(__pyx_k__7), 0, 1, 0, 0},
     {&__pyx_n_s_ability_dice, __pyx_k_ability_dice, sizeof(__pyx_k_ability_dice), 0, 0, 1, 1},
@@ -28042,14 +28611,16 @@
     {&__pyx_n_s_genexpr, __pyx_k_genexpr, sizeof(__pyx_k_genexpr), 0, 0, 1, 1},
     {&__pyx_n_s_geometric_variate, __pyx_k_geometric_variate, sizeof(__pyx_k_geometric_variate), 0, 0, 1, 1},
     {&__pyx_n_s_get_answer, __pyx_k_get_answer, sizeof(__pyx_k_get_answer), 0, 0, 1, 1},
     {&__pyx_n_s_hi, __pyx_k_hi, sizeof(__pyx_k_hi), 0, 0, 1, 1},
     {&__pyx_n_s_high, __pyx_k_high, sizeof(__pyx_k_high), 0, 0, 1, 1},
     {&__pyx_n_s_i, __pyx_k_i, sizeof(__pyx_k_i), 0, 0, 1, 1},
     {&__pyx_n_s_import, __pyx_k_import, sizeof(__pyx_k_import), 0, 0, 1, 1},
+    {&__pyx_n_s_index, __pyx_k_index, sizeof(__pyx_k_index), 0, 0, 1, 1},
+    {&__pyx_n_u_index, __pyx_k_index, sizeof(__pyx_k_index), 0, 1, 0, 1},
     {&__pyx_n_s_init, __pyx_k_init, sizeof(__pyx_k_init), 0, 0, 1, 1},
     {&__pyx_n_s_init_subclass, __pyx_k_init_subclass, sizeof(__pyx_k_init_subclass), 0, 0, 1, 1},
     {&__pyx_n_s_input, __pyx_k_input, sizeof(__pyx_k_input), 0, 0, 1, 1},
     {&__pyx_n_s_int, __pyx_k_int, sizeof(__pyx_k_int), 0, 0, 1, 1},
     {&__pyx_n_s_is_coroutine, __pyx_k_is_coroutine, sizeof(__pyx_k_is_coroutine), 0, 0, 1, 1},
     {&__pyx_kp_u_isenabled, __pyx_k_isenabled, sizeof(__pyx_k_isenabled), 0, 1, 0, 0},
     {&__pyx_n_s_items, __pyx_k_items, sizeof(__pyx_k_items), 0, 0, 1, 1},
@@ -28107,14 +28678,16 @@
     {&__pyx_n_s_normal_variate, __pyx_k_normal_variate, sizeof(__pyx_k_normal_variate), 0, 0, 1, 1},
     {&__pyx_n_s_number, __pyx_k_number, sizeof(__pyx_k_number), 0, 0, 1, 1},
     {&__pyx_n_s_number_of_trials, __pyx_k_number_of_trials, sizeof(__pyx_k_number_of_trials), 0, 0, 1, 1},
     {&__pyx_n_s_optimized_data, __pyx_k_optimized_data, sizeof(__pyx_k_optimized_data), 0, 0, 1, 1},
     {&__pyx_n_s_options, __pyx_k_options, sizeof(__pyx_k_options), 0, 0, 1, 1},
     {&__pyx_n_s_pareto_variate, __pyx_k_pareto_variate, sizeof(__pyx_k_pareto_variate), 0, 0, 1, 1},
     {&__pyx_n_s_percent_true, __pyx_k_percent_true, sizeof(__pyx_k_percent_true), 0, 0, 1, 1},
+    {&__pyx_n_s_pivot, __pyx_k_pivot, sizeof(__pyx_k_pivot), 0, 0, 1, 1},
+    {&__pyx_n_u_pivot, __pyx_k_pivot, sizeof(__pyx_k_pivot), 0, 1, 0, 1},
     {&__pyx_n_s_plus_or_minus, __pyx_k_plus_or_minus, sizeof(__pyx_k_plus_or_minus), 0, 0, 1, 1},
     {&__pyx_n_s_plus_or_minus_gauss, __pyx_k_plus_or_minus_gauss, sizeof(__pyx_k_plus_or_minus_gauss), 0, 0, 1, 1},
     {&__pyx_n_s_plus_or_minus_linear, __pyx_k_plus_or_minus_linear, sizeof(__pyx_k_plus_or_minus_linear), 0, 0, 1, 1},
     {&__pyx_n_s_poisson_variate, __pyx_k_poisson_variate, sizeof(__pyx_k_poisson_variate), 0, 0, 1, 1},
     {&__pyx_n_s_population, __pyx_k_population, sizeof(__pyx_k_population), 0, 0, 1, 1},
     {&__pyx_n_s_prepare, __pyx_k_prepare, sizeof(__pyx_k_prepare), 0, 0, 1, 1},
     {&__pyx_n_s_prev_weight, __pyx_k_prev_weight, sizeof(__pyx_k_prev_weight), 0, 0, 1, 1},
@@ -28213,17 +28786,17 @@
 }
 /* #### Code section: cached_builtins ### */
 static CYTHON_SMALL_CODE int __Pyx_InitCachedBuiltins(void) {
   __pyx_builtin_TypeError = __Pyx_GetBuiltinName(__pyx_n_s_TypeError); if (!__pyx_builtin_TypeError) __PYX_ERR(0, 336, __pyx_L1_error)
   __pyx_builtin_reversed = __Pyx_GetBuiltinName(__pyx_n_s_reversed); if (!__pyx_builtin_reversed) __PYX_ERR(0, 348, __pyx_L1_error)
   __pyx_builtin_range = __Pyx_GetBuiltinName(__pyx_n_s_range); if (!__pyx_builtin_range) __PYX_ERR(0, 348, __pyx_L1_error)
   __pyx_builtin_AssertionError = __Pyx_GetBuiltinName(__pyx_n_s_AssertionError); if (!__pyx_builtin_AssertionError) __PYX_ERR(0, 504, __pyx_L1_error)
-  __pyx_builtin_sorted = __Pyx_GetBuiltinName(__pyx_n_s_sorted); if (!__pyx_builtin_sorted) __PYX_ERR(0, 837, __pyx_L1_error)
-  __pyx_builtin_enumerate = __Pyx_GetBuiltinName(__pyx_n_s_enumerate); if (!__pyx_builtin_enumerate) __PYX_ERR(0, 908, __pyx_L1_error)
-  __pyx_builtin_input = __Pyx_GetBuiltinName(__pyx_n_s_input); if (!__pyx_builtin_input) __PYX_ERR(0, 917, __pyx_L1_error)
+  __pyx_builtin_sorted = __Pyx_GetBuiltinName(__pyx_n_s_sorted); if (!__pyx_builtin_sorted) __PYX_ERR(0, 852, __pyx_L1_error)
+  __pyx_builtin_enumerate = __Pyx_GetBuiltinName(__pyx_n_s_enumerate); if (!__pyx_builtin_enumerate) __PYX_ERR(0, 923, __pyx_L1_error)
+  __pyx_builtin_input = __Pyx_GetBuiltinName(__pyx_n_s_input); if (!__pyx_builtin_input) __PYX_ERR(0, 932, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
 /* #### Code section: cached_constants ### */
 
 static CYTHON_SMALL_CODE int __Pyx_InitCachedConstants(void) {
@@ -28786,551 +29359,580 @@
  * 
  */
   __pyx_tuple__83 = PyTuple_Pack(3, __pyx_n_s_self, __pyx_n_s_args, __pyx_n_s_kwargs); if (unlikely(!__pyx_tuple__83)) __PYX_ERR(0, 548, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__83);
   __Pyx_GIVEREF(__pyx_tuple__83);
   __pyx_codeobj__84 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS|CO_VARARGS|CO_VARKEYWORDS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__83, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_Fortuna_pyx, __pyx_n_s_call, 548, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__84)) __PYX_ERR(0, 548, __pyx_L1_error)
 
-  /* "Fortuna.pyx":581
- *     Please refer to https://pypi.org/project/Fortuna/ for full documentation.
- *     """
- *     __slots__ = ("flat", "data", "rotate_size")             # <<<<<<<<<<<<<<
+  /* "Fortuna.pyx":553
+ * 
+ * class TruffleShuffle2:
+ *     __slots__ = ("flat", "data", "size", "pivot", "index")             # <<<<<<<<<<<<<<
  * 
  *     def __init__(self, collection: Iterable, flat: bool = True):
  */
-  __pyx_tuple__85 = PyTuple_Pack(3, __pyx_n_u_flat, __pyx_n_u_data, __pyx_n_u_rotate_size); if (unlikely(!__pyx_tuple__85)) __PYX_ERR(0, 581, __pyx_L1_error)
+  __pyx_tuple__85 = PyTuple_Pack(5, __pyx_n_u_flat, __pyx_n_u_data, __pyx_n_u_size, __pyx_n_u_pivot, __pyx_n_u_index); if (unlikely(!__pyx_tuple__85)) __PYX_ERR(0, 553, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__85);
   __Pyx_GIVEREF(__pyx_tuple__85);
 
-  /* "Fortuna.pyx":583
- *     __slots__ = ("flat", "data", "rotate_size")
+  /* "Fortuna.pyx":555
+ *     __slots__ = ("flat", "data", "size", "pivot", "index")
  * 
  *     def __init__(self, collection: Iterable, flat: bool = True):             # <<<<<<<<<<<<<<
  *         self.flat = flat
- *         data = list(collection)
+ *         self.data = list(collection) if isinstance(collection, Iterator) else collection
  */
-  __pyx_tuple__86 = PyTuple_Pack(4, __pyx_n_s_self, __pyx_n_s_collection, __pyx_n_s_flat, __pyx_n_s_data); if (unlikely(!__pyx_tuple__86)) __PYX_ERR(0, 583, __pyx_L1_error)
+  __pyx_tuple__86 = PyTuple_Pack(3, __pyx_n_s_self, __pyx_n_s_collection, __pyx_n_s_flat); if (unlikely(!__pyx_tuple__86)) __PYX_ERR(0, 555, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__86);
   __Pyx_GIVEREF(__pyx_tuple__86);
-  __pyx_codeobj__87 = (PyObject*)__Pyx_PyCode_New(3, 0, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__86, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_Fortuna_pyx, __pyx_n_s_init, 583, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__87)) __PYX_ERR(0, 583, __pyx_L1_error)
-  __pyx_tuple__88 = PyTuple_Pack(1, ((PyObject *)Py_True)); if (unlikely(!__pyx_tuple__88)) __PYX_ERR(0, 583, __pyx_L1_error)
+  __pyx_codeobj__87 = (PyObject*)__Pyx_PyCode_New(3, 0, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__86, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_Fortuna_pyx, __pyx_n_s_init, 555, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__87)) __PYX_ERR(0, 555, __pyx_L1_error)
+  __pyx_tuple__88 = PyTuple_Pack(1, ((PyObject *)Py_True)); if (unlikely(!__pyx_tuple__88)) __PYX_ERR(0, 555, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__88);
   __Pyx_GIVEREF(__pyx_tuple__88);
 
-  /* "Fortuna.pyx":590
+  /* "Fortuna.pyx":562
+ *         self.index = _random_index(self.size)
+ * 
+ *     def __call__(self, *args, **kwargs):             # <<<<<<<<<<<<<<
+ *         self.index = (self.index + 1 + _front_poisson(self.pivot)) % self.size
+ *         return flatten(self.data[self.index], *args, flat=self.flat, **kwargs)
+ */
+  __pyx_codeobj__89 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS|CO_VARARGS|CO_VARKEYWORDS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__83, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_Fortuna_pyx, __pyx_n_s_call, 562, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__89)) __PYX_ERR(0, 562, __pyx_L1_error)
+
+  /* "Fortuna.pyx":596
+ *     Please refer to https://pypi.org/project/Fortuna/ for full documentation.
+ *     """
+ *     __slots__ = ("flat", "data", "rotate_size")             # <<<<<<<<<<<<<<
+ * 
+ *     def __init__(self, collection: Iterable, flat: bool = True):
+ */
+  __pyx_tuple__90 = PyTuple_Pack(3, __pyx_n_u_flat, __pyx_n_u_data, __pyx_n_u_rotate_size); if (unlikely(!__pyx_tuple__90)) __PYX_ERR(0, 596, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__90);
+  __Pyx_GIVEREF(__pyx_tuple__90);
+
+  /* "Fortuna.pyx":598
+ *     __slots__ = ("flat", "data", "rotate_size")
+ * 
+ *     def __init__(self, collection: Iterable, flat: bool = True):             # <<<<<<<<<<<<<<
+ *         self.flat = flat
+ *         data = list(collection)
+ */
+  __pyx_tuple__91 = PyTuple_Pack(4, __pyx_n_s_self, __pyx_n_s_collection, __pyx_n_s_flat, __pyx_n_s_data); if (unlikely(!__pyx_tuple__91)) __PYX_ERR(0, 598, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__91);
+  __Pyx_GIVEREF(__pyx_tuple__91);
+  __pyx_codeobj__92 = (PyObject*)__Pyx_PyCode_New(3, 0, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__91, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_Fortuna_pyx, __pyx_n_s_init, 598, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__92)) __PYX_ERR(0, 598, __pyx_L1_error)
+
+  /* "Fortuna.pyx":605
  *         self.rotate_size = int(sqrt(len(self.data)))
  * 
  *     def __call__(self, *args, **kwargs):             # <<<<<<<<<<<<<<
  *         self.data.rotate(1 + _front_poisson(self.rotate_size))
  *         return flatten(self.data[-1], *args, flat=self.flat, **kwargs)
  */
-  __pyx_codeobj__89 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS|CO_VARARGS|CO_VARKEYWORDS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__83, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_Fortuna_pyx, __pyx_n_s_call, 590, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__89)) __PYX_ERR(0, 590, __pyx_L1_error)
+  __pyx_codeobj__93 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS|CO_VARARGS|CO_VARKEYWORDS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__83, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_Fortuna_pyx, __pyx_n_s_call, 605, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__93)) __PYX_ERR(0, 605, __pyx_L1_error)
 
-  /* "Fortuna.pyx":608
+  /* "Fortuna.pyx":623
  *     Please refer to https://pypi.org/project/Fortuna/ for full documentation.
  *     """
  *     __slots__ = ("flat", "size", "data", "truffle_shuffle", "cycles")             # <<<<<<<<<<<<<<
  * 
  *     def __init__(self, collection: Iterable, flat: bool = True):
  */
-  __pyx_tuple__90 = PyTuple_Pack(5, __pyx_n_u_flat, __pyx_n_u_size, __pyx_n_u_data, __pyx_n_u_truffle_shuffle, __pyx_n_u_cycles); if (unlikely(!__pyx_tuple__90)) __PYX_ERR(0, 608, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__90);
-  __Pyx_GIVEREF(__pyx_tuple__90);
+  __pyx_tuple__94 = PyTuple_Pack(5, __pyx_n_u_flat, __pyx_n_u_size, __pyx_n_u_data, __pyx_n_u_truffle_shuffle, __pyx_n_u_cycles); if (unlikely(!__pyx_tuple__94)) __PYX_ERR(0, 623, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__94);
+  __Pyx_GIVEREF(__pyx_tuple__94);
 
-  /* "Fortuna.pyx":610
+  /* "Fortuna.pyx":625
  *     __slots__ = ("flat", "size", "data", "truffle_shuffle", "cycles")
  * 
  *     def __init__(self, collection: Iterable, flat: bool = True):             # <<<<<<<<<<<<<<
  *         self.flat = flat
  *         self.data = tuple(collection)
  */
-  __pyx_tuple__91 = PyTuple_Pack(3, __pyx_n_s_self, __pyx_n_s_collection, __pyx_n_s_flat); if (unlikely(!__pyx_tuple__91)) __PYX_ERR(0, 610, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__91);
-  __Pyx_GIVEREF(__pyx_tuple__91);
-  __pyx_codeobj__92 = (PyObject*)__Pyx_PyCode_New(3, 0, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__91, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_Fortuna_pyx, __pyx_n_s_init, 610, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__92)) __PYX_ERR(0, 610, __pyx_L1_error)
+  __pyx_codeobj__95 = (PyObject*)__Pyx_PyCode_New(3, 0, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__86, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_Fortuna_pyx, __pyx_n_s_init, 625, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__95)) __PYX_ERR(0, 625, __pyx_L1_error)
 
-  /* "Fortuna.pyx":618
+  /* "Fortuna.pyx":633
  *         self.truffle_shuffle = TruffleShuffle(self.data, flat)
  * 
  *     def __call__(self, *args, **kwargs):             # <<<<<<<<<<<<<<
  *         return self.quantum_monty(*args, **kwargs)
  * 
  */
-  __pyx_codeobj__93 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS|CO_VARARGS|CO_VARKEYWORDS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__83, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_Fortuna_pyx, __pyx_n_s_call, 618, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__93)) __PYX_ERR(0, 618, __pyx_L1_error)
+  __pyx_codeobj__96 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS|CO_VARARGS|CO_VARKEYWORDS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__83, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_Fortuna_pyx, __pyx_n_s_call, 633, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__96)) __PYX_ERR(0, 633, __pyx_L1_error)
 
-  /* "Fortuna.pyx":621
+  /* "Fortuna.pyx":636
  *         return self.quantum_monty(*args, **kwargs)
  * 
  *     def dispatch(self, monty: str) -> Callable:             # <<<<<<<<<<<<<<
  *         """ For dispatch automation.
  *         In general, prefer to use the methods directly when possible. """
  */
-  __pyx_tuple__94 = PyTuple_Pack(2, __pyx_n_s_self, __pyx_n_s_monty); if (unlikely(!__pyx_tuple__94)) __PYX_ERR(0, 621, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__94);
-  __Pyx_GIVEREF(__pyx_tuple__94);
-  __pyx_codeobj__95 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__94, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_Fortuna_pyx, __pyx_n_s_dispatch, 621, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__95)) __PYX_ERR(0, 621, __pyx_L1_error)
+  __pyx_tuple__97 = PyTuple_Pack(2, __pyx_n_s_self, __pyx_n_s_monty); if (unlikely(!__pyx_tuple__97)) __PYX_ERR(0, 636, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__97);
+  __Pyx_GIVEREF(__pyx_tuple__97);
+  __pyx_codeobj__98 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__97, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_Fortuna_pyx, __pyx_n_s_dispatch, 636, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__98)) __PYX_ERR(0, 636, __pyx_L1_error)
 
-  /* "Fortuna.pyx":643
+  /* "Fortuna.pyx":658
  *         }[monty]
  * 
  *     def flat_uniform(self, *args, **kwargs):             # <<<<<<<<<<<<<<
  *         return flatten(
  *             self.data[_random_index(self.size)], *args, flat=self.flat, **kwargs
  */
-  __pyx_codeobj__96 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS|CO_VARARGS|CO_VARKEYWORDS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__83, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_Fortuna_pyx, __pyx_n_s_flat_uniform, 643, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__96)) __PYX_ERR(0, 643, __pyx_L1_error)
+  __pyx_codeobj__99 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS|CO_VARARGS|CO_VARKEYWORDS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__83, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_Fortuna_pyx, __pyx_n_s_flat_uniform, 658, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__99)) __PYX_ERR(0, 658, __pyx_L1_error)
 
-  /* "Fortuna.pyx":648
+  /* "Fortuna.pyx":663
  *         )
  * 
  *     def cycle(self, *args, **kwargs):             # <<<<<<<<<<<<<<
  *         return flatten(
  *             next(self.cycles), *args, flat=self.flat, **kwargs
  */
-  __pyx_codeobj__97 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS|CO_VARARGS|CO_VARKEYWORDS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__83, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_Fortuna_pyx, __pyx_n_s_cycle, 648, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__97)) __PYX_ERR(0, 648, __pyx_L1_error)
+  __pyx_codeobj__100 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS|CO_VARARGS|CO_VARKEYWORDS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__83, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_Fortuna_pyx, __pyx_n_s_cycle, 663, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__100)) __PYX_ERR(0, 663, __pyx_L1_error)
 
-  /* "Fortuna.pyx":653
+  /* "Fortuna.pyx":668
  *         )
  * 
  *     def front_linear(self, *args, **kwargs):             # <<<<<<<<<<<<<<
  *         return flatten(
  *             self.data[_front_linear(self.size)], *args, flat=self.flat, **kwargs
  */
-  __pyx_codeobj__98 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS|CO_VARARGS|CO_VARKEYWORDS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__83, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_Fortuna_pyx, __pyx_n_s_front_linear, 653, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__98)) __PYX_ERR(0, 653, __pyx_L1_error)
+  __pyx_codeobj__101 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS|CO_VARARGS|CO_VARKEYWORDS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__83, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_Fortuna_pyx, __pyx_n_s_front_linear, 668, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__101)) __PYX_ERR(0, 668, __pyx_L1_error)
 
-  /* "Fortuna.pyx":658
+  /* "Fortuna.pyx":673
  *         )
  * 
  *     def middle_linear(self, *args, **kwargs):             # <<<<<<<<<<<<<<
  *         return flatten(
  *             self.data[_middle_linear(self.size)], *args, flat=self.flat, **kwargs
  */
-  __pyx_codeobj__99 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS|CO_VARARGS|CO_VARKEYWORDS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__83, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_Fortuna_pyx, __pyx_n_s_middle_linear, 658, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__99)) __PYX_ERR(0, 658, __pyx_L1_error)
+  __pyx_codeobj__102 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS|CO_VARARGS|CO_VARKEYWORDS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__83, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_Fortuna_pyx, __pyx_n_s_middle_linear, 673, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__102)) __PYX_ERR(0, 673, __pyx_L1_error)
 
-  /* "Fortuna.pyx":663
+  /* "Fortuna.pyx":678
  *         )
  * 
  *     def back_linear(self, *args, **kwargs):             # <<<<<<<<<<<<<<
  *         return flatten(
  *             self.data[_back_linear(self.size)], *args, flat=self.flat, **kwargs
  */
-  __pyx_codeobj__100 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS|CO_VARARGS|CO_VARKEYWORDS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__83, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_Fortuna_pyx, __pyx_n_s_back_linear, 663, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__100)) __PYX_ERR(0, 663, __pyx_L1_error)
+  __pyx_codeobj__103 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS|CO_VARARGS|CO_VARKEYWORDS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__83, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_Fortuna_pyx, __pyx_n_s_back_linear, 678, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__103)) __PYX_ERR(0, 678, __pyx_L1_error)
 
-  /* "Fortuna.pyx":668
+  /* "Fortuna.pyx":683
  *         )
  * 
  *     def quantum_linear(self, *args, **kwargs):             # <<<<<<<<<<<<<<
  *         return flatten(
  *             self.data[_quantum_linear(self.size)], *args, flat=self.flat, **kwargs
  */
-  __pyx_codeobj__101 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS|CO_VARARGS|CO_VARKEYWORDS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__83, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_Fortuna_pyx, __pyx_n_s_quantum_linear, 668, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__101)) __PYX_ERR(0, 668, __pyx_L1_error)
+  __pyx_codeobj__104 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS|CO_VARARGS|CO_VARKEYWORDS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__83, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_Fortuna_pyx, __pyx_n_s_quantum_linear, 683, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__104)) __PYX_ERR(0, 683, __pyx_L1_error)
 
-  /* "Fortuna.pyx":673
+  /* "Fortuna.pyx":688
  *         )
  * 
  *     def front_gauss(self, *args, **kwargs):             # <<<<<<<<<<<<<<
  *         return flatten(
  *             self.data[_front_gauss(self.size)], *args, flat=self.flat, **kwargs)
  */
-  __pyx_codeobj__102 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS|CO_VARARGS|CO_VARKEYWORDS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__83, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_Fortuna_pyx, __pyx_n_s_front_gauss, 673, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__102)) __PYX_ERR(0, 673, __pyx_L1_error)
+  __pyx_codeobj__105 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS|CO_VARARGS|CO_VARKEYWORDS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__83, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_Fortuna_pyx, __pyx_n_s_front_gauss, 688, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__105)) __PYX_ERR(0, 688, __pyx_L1_error)
 
-  /* "Fortuna.pyx":677
+  /* "Fortuna.pyx":692
  *             self.data[_front_gauss(self.size)], *args, flat=self.flat, **kwargs)
  * 
  *     def middle_gauss(self, *args, **kwargs):             # <<<<<<<<<<<<<<
  *         return flatten(
  *             self.data[_middle_gauss(self.size)], *args, flat=self.flat, **kwargs
  */
-  __pyx_codeobj__103 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS|CO_VARARGS|CO_VARKEYWORDS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__83, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_Fortuna_pyx, __pyx_n_s_middle_gauss, 677, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__103)) __PYX_ERR(0, 677, __pyx_L1_error)
+  __pyx_codeobj__106 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS|CO_VARARGS|CO_VARKEYWORDS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__83, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_Fortuna_pyx, __pyx_n_s_middle_gauss, 692, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__106)) __PYX_ERR(0, 692, __pyx_L1_error)
 
-  /* "Fortuna.pyx":682
+  /* "Fortuna.pyx":697
  *         )
  * 
  *     def back_gauss(self, *args, **kwargs):             # <<<<<<<<<<<<<<
  *         return flatten(
  *             self.data[_back_gauss(self.size)], *args, flat=self.flat, **kwargs
  */
-  __pyx_codeobj__104 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS|CO_VARARGS|CO_VARKEYWORDS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__83, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_Fortuna_pyx, __pyx_n_s_back_gauss, 682, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__104)) __PYX_ERR(0, 682, __pyx_L1_error)
+  __pyx_codeobj__107 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS|CO_VARARGS|CO_VARKEYWORDS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__83, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_Fortuna_pyx, __pyx_n_s_back_gauss, 697, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__107)) __PYX_ERR(0, 697, __pyx_L1_error)
 
-  /* "Fortuna.pyx":687
+  /* "Fortuna.pyx":702
  *         )
  * 
  *     def quantum_gauss(self, *args, **kwargs):             # <<<<<<<<<<<<<<
  *         return flatten(
  *             self.data[_quantum_gauss(self.size)], *args, flat=self.flat, **kwargs
  */
-  __pyx_codeobj__105 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS|CO_VARARGS|CO_VARKEYWORDS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__83, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_Fortuna_pyx, __pyx_n_s_quantum_gauss, 687, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__105)) __PYX_ERR(0, 687, __pyx_L1_error)
+  __pyx_codeobj__108 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS|CO_VARARGS|CO_VARKEYWORDS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__83, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_Fortuna_pyx, __pyx_n_s_quantum_gauss, 702, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__108)) __PYX_ERR(0, 702, __pyx_L1_error)
 
-  /* "Fortuna.pyx":692
+  /* "Fortuna.pyx":707
  *         )
  * 
  *     def front_poisson(self, *args, **kwargs):             # <<<<<<<<<<<<<<
  *         return flatten(
  *             self.data[_front_poisson(self.size)], *args, flat=self.flat, **kwargs
  */
-  __pyx_codeobj__106 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS|CO_VARARGS|CO_VARKEYWORDS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__83, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_Fortuna_pyx, __pyx_n_s_front_poisson, 692, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__106)) __PYX_ERR(0, 692, __pyx_L1_error)
+  __pyx_codeobj__109 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS|CO_VARARGS|CO_VARKEYWORDS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__83, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_Fortuna_pyx, __pyx_n_s_front_poisson, 707, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__109)) __PYX_ERR(0, 707, __pyx_L1_error)
 
-  /* "Fortuna.pyx":697
+  /* "Fortuna.pyx":712
  *         )
  * 
  *     def middle_poisson(self, *args, **kwargs):             # <<<<<<<<<<<<<<
  *         return flatten(
  *             self.data[_middle_poisson(self.size)], *args, flat=self.flat, **kwargs
  */
-  __pyx_codeobj__107 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS|CO_VARARGS|CO_VARKEYWORDS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__83, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_Fortuna_pyx, __pyx_n_s_middle_poisson, 697, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__107)) __PYX_ERR(0, 697, __pyx_L1_error)
+  __pyx_codeobj__110 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS|CO_VARARGS|CO_VARKEYWORDS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__83, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_Fortuna_pyx, __pyx_n_s_middle_poisson, 712, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__110)) __PYX_ERR(0, 712, __pyx_L1_error)
 
-  /* "Fortuna.pyx":702
+  /* "Fortuna.pyx":717
  *         )
  * 
  *     def back_poisson(self, *args, **kwargs):             # <<<<<<<<<<<<<<
  *         return flatten(
  *             self.data[_back_poisson(self.size)], *args, flat=self.flat, **kwargs
  */
-  __pyx_codeobj__108 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS|CO_VARARGS|CO_VARKEYWORDS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__83, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_Fortuna_pyx, __pyx_n_s_back_poisson, 702, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__108)) __PYX_ERR(0, 702, __pyx_L1_error)
+  __pyx_codeobj__111 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS|CO_VARARGS|CO_VARKEYWORDS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__83, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_Fortuna_pyx, __pyx_n_s_back_poisson, 717, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__111)) __PYX_ERR(0, 717, __pyx_L1_error)
 
-  /* "Fortuna.pyx":707
+  /* "Fortuna.pyx":722
  *         )
  * 
  *     def quantum_poisson(self, *args, **kwargs):             # <<<<<<<<<<<<<<
  *         return flatten(
  *             self.data[_quantum_poisson(self.size)], *args, flat=self.flat, **kwargs
  */
-  __pyx_codeobj__109 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS|CO_VARARGS|CO_VARKEYWORDS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__83, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_Fortuna_pyx, __pyx_n_s_quantum_poisson, 707, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__109)) __PYX_ERR(0, 707, __pyx_L1_error)
+  __pyx_codeobj__112 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS|CO_VARARGS|CO_VARKEYWORDS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__83, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_Fortuna_pyx, __pyx_n_s_quantum_poisson, 722, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__112)) __PYX_ERR(0, 722, __pyx_L1_error)
 
-  /* "Fortuna.pyx":712
+  /* "Fortuna.pyx":727
  *         )
  * 
  *     def quantum_monty(self, *args, **kwargs):             # <<<<<<<<<<<<<<
  *         return flatten(
  *             self.data[_quantum_monty(self.size)], *args, flat=self.flat, **kwargs
  */
-  __pyx_codeobj__110 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS|CO_VARARGS|CO_VARKEYWORDS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__83, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_Fortuna_pyx, __pyx_n_s_quantum_monty, 712, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__110)) __PYX_ERR(0, 712, __pyx_L1_error)
+  __pyx_codeobj__113 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS|CO_VARARGS|CO_VARKEYWORDS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__83, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_Fortuna_pyx, __pyx_n_s_quantum_monty, 727, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__113)) __PYX_ERR(0, 727, __pyx_L1_error)
 
-  /* "Fortuna.pyx":738
+  /* "Fortuna.pyx":753
  *     Please refer to https://pypi.org/project/Fortuna/ for full documentation.
  *     """
  *     __slots__ = ("random_cat", "random_selection", "cat_keys", "matrix_data",             # <<<<<<<<<<<<<<
  *                  "double_cycle", "cycle")
  * 
  */
-  __pyx_tuple__111 = PyTuple_Pack(6, __pyx_n_u_random_cat, __pyx_n_u_random_selection, __pyx_n_u_cat_keys, __pyx_n_u_matrix_data, __pyx_n_u_double_cycle, __pyx_n_u_cycle); if (unlikely(!__pyx_tuple__111)) __PYX_ERR(0, 738, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__111);
-  __Pyx_GIVEREF(__pyx_tuple__111);
+  __pyx_tuple__114 = PyTuple_Pack(6, __pyx_n_u_random_cat, __pyx_n_u_random_selection, __pyx_n_u_cat_keys, __pyx_n_u_matrix_data, __pyx_n_u_double_cycle, __pyx_n_u_cycle); if (unlikely(!__pyx_tuple__114)) __PYX_ERR(0, 753, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__114);
+  __Pyx_GIVEREF(__pyx_tuple__114);
 
-  /* "Fortuna.pyx":741
+  /* "Fortuna.pyx":756
  *                  "double_cycle", "cycle")
  * 
  *     def __init__(self,             # <<<<<<<<<<<<<<
  *                  matrix_data: Dict,
  *                  key_bias: str = "front_linear",
  */
-  __pyx_tuple__112 = PyTuple_Pack(9, __pyx_n_s_self, __pyx_n_s_matrix_data, __pyx_n_s_key_bias, __pyx_n_s_val_bias, __pyx_n_s_flat, __pyx_n_s_cycle_source, __pyx_n_s_seq, __pyx_n_s_key, __pyx_n_s_seq); if (unlikely(!__pyx_tuple__112)) __PYX_ERR(0, 741, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__112);
-  __Pyx_GIVEREF(__pyx_tuple__112);
-  __pyx_codeobj__113 = (PyObject*)__Pyx_PyCode_New(5, 0, 0, 9, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__112, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_Fortuna_pyx, __pyx_n_s_init, 741, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__113)) __PYX_ERR(0, 741, __pyx_L1_error)
-  __pyx_tuple__114 = PyTuple_Pack(3, ((PyObject*)__pyx_n_u_front_linear), ((PyObject*)__pyx_n_u_truffle_shuffle), ((PyObject *)Py_True)); if (unlikely(!__pyx_tuple__114)) __PYX_ERR(0, 741, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__114);
-  __Pyx_GIVEREF(__pyx_tuple__114);
+  __pyx_tuple__115 = PyTuple_Pack(9, __pyx_n_s_self, __pyx_n_s_matrix_data, __pyx_n_s_key_bias, __pyx_n_s_val_bias, __pyx_n_s_flat, __pyx_n_s_cycle_source, __pyx_n_s_seq, __pyx_n_s_key, __pyx_n_s_seq); if (unlikely(!__pyx_tuple__115)) __PYX_ERR(0, 756, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__115);
+  __Pyx_GIVEREF(__pyx_tuple__115);
+  __pyx_codeobj__116 = (PyObject*)__Pyx_PyCode_New(5, 0, 0, 9, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__115, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_Fortuna_pyx, __pyx_n_s_init, 756, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__116)) __PYX_ERR(0, 756, __pyx_L1_error)
+  __pyx_tuple__117 = PyTuple_Pack(3, ((PyObject*)__pyx_n_u_front_linear), ((PyObject*)__pyx_n_u_truffle_shuffle), ((PyObject *)Py_True)); if (unlikely(!__pyx_tuple__117)) __PYX_ERR(0, 756, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__117);
+  __Pyx_GIVEREF(__pyx_tuple__117);
 
-  /* "Fortuna.pyx":775
+  /* "Fortuna.pyx":790
  *         self.cycle = cycle(cycle_source)
  * 
  *     def __call__(self, cat_key=None, *args, **kwargs):             # <<<<<<<<<<<<<<
  *         """
  *         @param cat_key : Optional String. Default is None.
  */
-  __pyx_tuple__115 = PyTuple_Pack(6, __pyx_n_s_self, __pyx_n_s_cat_key, __pyx_n_s_args, __pyx_n_s_kwargs, __pyx_n_s_monty, __pyx_n_s_key); if (unlikely(!__pyx_tuple__115)) __PYX_ERR(0, 775, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__115);
-  __Pyx_GIVEREF(__pyx_tuple__115);
-  __pyx_codeobj__116 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 6, 0, CO_OPTIMIZED|CO_NEWLOCALS|CO_VARARGS|CO_VARKEYWORDS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__115, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_Fortuna_pyx, __pyx_n_s_call, 775, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__116)) __PYX_ERR(0, 775, __pyx_L1_error)
-  __pyx_tuple__117 = PyTuple_Pack(1, Py_None); if (unlikely(!__pyx_tuple__117)) __PYX_ERR(0, 775, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__117);
-  __Pyx_GIVEREF(__pyx_tuple__117);
+  __pyx_tuple__118 = PyTuple_Pack(6, __pyx_n_s_self, __pyx_n_s_cat_key, __pyx_n_s_args, __pyx_n_s_kwargs, __pyx_n_s_monty, __pyx_n_s_key); if (unlikely(!__pyx_tuple__118)) __PYX_ERR(0, 790, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__118);
+  __Pyx_GIVEREF(__pyx_tuple__118);
+  __pyx_codeobj__119 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 6, 0, CO_OPTIMIZED|CO_NEWLOCALS|CO_VARARGS|CO_VARKEYWORDS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__118, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_Fortuna_pyx, __pyx_n_s_call, 790, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__119)) __PYX_ERR(0, 790, __pyx_L1_error)
+  __pyx_tuple__120 = PyTuple_Pack(1, Py_None); if (unlikely(!__pyx_tuple__120)) __PYX_ERR(0, 790, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__120);
+  __Pyx_GIVEREF(__pyx_tuple__120);
 
-  /* "Fortuna.pyx":807
+  /* "Fortuna.pyx":822
  *     Please refer to https://pypi.org/project/Fortuna/ for full documentation.
  *     """
  *     __slots__ = ("flat", "max_weight", "data")             # <<<<<<<<<<<<<<
  * 
  *     def __call__(self, *args, **kwargs):
  */
-  __pyx_tuple__118 = PyTuple_Pack(3, __pyx_n_u_flat, __pyx_n_u_max_weight, __pyx_n_u_data); if (unlikely(!__pyx_tuple__118)) __PYX_ERR(0, 807, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__118);
-  __Pyx_GIVEREF(__pyx_tuple__118);
+  __pyx_tuple__121 = PyTuple_Pack(3, __pyx_n_u_flat, __pyx_n_u_max_weight, __pyx_n_u_data); if (unlikely(!__pyx_tuple__121)) __PYX_ERR(0, 822, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__121);
+  __Pyx_GIVEREF(__pyx_tuple__121);
 
-  /* "Fortuna.pyx":809
+  /* "Fortuna.pyx":824
  *     __slots__ = ("flat", "max_weight", "data")
  * 
  *     def __call__(self, *args, **kwargs):             # <<<<<<<<<<<<<<
  *         """
  *         @param *args, **kwargs : Optional arguments
  */
-  __pyx_tuple__119 = PyTuple_Pack(6, __pyx_n_s_self, __pyx_n_s_args, __pyx_n_s_kwargs, __pyx_n_s_rand, __pyx_n_s_weight, __pyx_n_s_value); if (unlikely(!__pyx_tuple__119)) __PYX_ERR(0, 809, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__119);
-  __Pyx_GIVEREF(__pyx_tuple__119);
-  __pyx_codeobj__120 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 6, 0, CO_OPTIMIZED|CO_NEWLOCALS|CO_VARARGS|CO_VARKEYWORDS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__119, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_Fortuna_pyx, __pyx_n_s_call, 809, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__120)) __PYX_ERR(0, 809, __pyx_L1_error)
+  __pyx_tuple__122 = PyTuple_Pack(6, __pyx_n_s_self, __pyx_n_s_args, __pyx_n_s_kwargs, __pyx_n_s_rand, __pyx_n_s_weight, __pyx_n_s_value); if (unlikely(!__pyx_tuple__122)) __PYX_ERR(0, 824, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__122);
+  __Pyx_GIVEREF(__pyx_tuple__122);
+  __pyx_codeobj__123 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 6, 0, CO_OPTIMIZED|CO_NEWLOCALS|CO_VARARGS|CO_VARKEYWORDS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__122, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_Fortuna_pyx, __pyx_n_s_call, 824, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__123)) __PYX_ERR(0, 824, __pyx_L1_error)
 
-  /* "Fortuna.pyx":826
+  /* "Fortuna.pyx":841
  *     __slots__ = ("flat", "max_weight", "data")
  * 
  *     def __init__(self,             # <<<<<<<<<<<<<<
  *                  weighted_table: Iterable,
  *                  flat: bool = True):
  */
-  __pyx_tuple__121 = PyTuple_Pack(9, __pyx_n_s_self, __pyx_n_s_weighted_table, __pyx_n_s_flat, __pyx_n_s_optimized_data, __pyx_n_s_cum_weight, __pyx_n_s_w_pair, __pyx_n_s_itm, __pyx_n_s_genexpr, __pyx_n_s_genexpr); if (unlikely(!__pyx_tuple__121)) __PYX_ERR(0, 826, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__121);
-  __Pyx_GIVEREF(__pyx_tuple__121);
-  __pyx_codeobj__122 = (PyObject*)__Pyx_PyCode_New(3, 0, 0, 9, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__121, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_Fortuna_pyx, __pyx_n_s_init, 826, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__122)) __PYX_ERR(0, 826, __pyx_L1_error)
+  __pyx_tuple__124 = PyTuple_Pack(9, __pyx_n_s_self, __pyx_n_s_weighted_table, __pyx_n_s_flat, __pyx_n_s_optimized_data, __pyx_n_s_cum_weight, __pyx_n_s_w_pair, __pyx_n_s_itm, __pyx_n_s_genexpr, __pyx_n_s_genexpr); if (unlikely(!__pyx_tuple__124)) __PYX_ERR(0, 841, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__124);
+  __Pyx_GIVEREF(__pyx_tuple__124);
+  __pyx_codeobj__125 = (PyObject*)__Pyx_PyCode_New(3, 0, 0, 9, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__124, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_Fortuna_pyx, __pyx_n_s_init, 841, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__125)) __PYX_ERR(0, 841, __pyx_L1_error)
 
-  /* "Fortuna.pyx":852
+  /* "Fortuna.pyx":867
  *     __slots__ = ("flat", "max_weight", "data")
  * 
  *     def __init__(self,             # <<<<<<<<<<<<<<
  *                  weighted_table: Iterable,
  *                  flat: bool = True):
  */
-  __pyx_tuple__123 = PyTuple_Pack(11, __pyx_n_s_self, __pyx_n_s_weighted_table, __pyx_n_s_flat, __pyx_n_s_data, __pyx_n_s_prev_weight, __pyx_n_s_w_pair, __pyx_n_s_optimized_data, __pyx_n_s_cum_weight, __pyx_n_s_itm, __pyx_n_s_genexpr, __pyx_n_s_genexpr); if (unlikely(!__pyx_tuple__123)) __PYX_ERR(0, 852, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__123);
-  __Pyx_GIVEREF(__pyx_tuple__123);
-  __pyx_codeobj__124 = (PyObject*)__Pyx_PyCode_New(3, 0, 0, 11, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__123, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_Fortuna_pyx, __pyx_n_s_init, 852, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__124)) __PYX_ERR(0, 852, __pyx_L1_error)
+  __pyx_tuple__126 = PyTuple_Pack(11, __pyx_n_s_self, __pyx_n_s_weighted_table, __pyx_n_s_flat, __pyx_n_s_data, __pyx_n_s_prev_weight, __pyx_n_s_w_pair, __pyx_n_s_optimized_data, __pyx_n_s_cum_weight, __pyx_n_s_itm, __pyx_n_s_genexpr, __pyx_n_s_genexpr); if (unlikely(!__pyx_tuple__126)) __PYX_ERR(0, 867, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__126);
+  __Pyx_GIVEREF(__pyx_tuple__126);
+  __pyx_codeobj__127 = (PyObject*)__Pyx_PyCode_New(3, 0, 0, 11, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__126, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_Fortuna_pyx, __pyx_n_s_init, 867, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__127)) __PYX_ERR(0, 867, __pyx_L1_error)
 
-  /* "Fortuna.pyx":881
+  /* "Fortuna.pyx":896
  *     MultiChoice: generates multiple choice style questions on the terminal. """
  * 
  *     def __init__(self,             # <<<<<<<<<<<<<<
  *                  query: str,
  *                  *,
  */
-  __pyx_tuple__125 = PyTuple_Pack(10, __pyx_n_s_self, __pyx_n_s_query, __pyx_n_s_options, __pyx_n_s_default, __pyx_n_s_strict, __pyx_n_s_cursor, __pyx_n_s_k, __pyx_n_s_v, __pyx_n_s_genexpr, __pyx_n_s_genexpr); if (unlikely(!__pyx_tuple__125)) __PYX_ERR(0, 881, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__125);
-  __Pyx_GIVEREF(__pyx_tuple__125);
-  __pyx_codeobj__126 = (PyObject*)__Pyx_PyCode_New(2, 0, 4, 10, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__125, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_Fortuna_pyx, __pyx_n_s_init, 881, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__126)) __PYX_ERR(0, 881, __pyx_L1_error)
+  __pyx_tuple__128 = PyTuple_Pack(10, __pyx_n_s_self, __pyx_n_s_query, __pyx_n_s_options, __pyx_n_s_default, __pyx_n_s_strict, __pyx_n_s_cursor, __pyx_n_s_k, __pyx_n_s_v, __pyx_n_s_genexpr, __pyx_n_s_genexpr); if (unlikely(!__pyx_tuple__128)) __PYX_ERR(0, 896, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__128);
+  __Pyx_GIVEREF(__pyx_tuple__128);
+  __pyx_codeobj__129 = (PyObject*)__Pyx_PyCode_New(2, 0, 4, 10, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__128, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_Fortuna_pyx, __pyx_n_s_init, 896, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__129)) __PYX_ERR(0, 896, __pyx_L1_error)
 
-  /* "Fortuna.pyx":916
+  /* "Fortuna.pyx":931
  *         )
  * 
  *     def _get_answer(self) -> str:             # <<<<<<<<<<<<<<
  *         return input('\n'.join(self.choice_pack)).lower() or self.default
  * 
  */
-  __pyx_codeobj__127 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__22, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_Fortuna_pyx, __pyx_n_s_get_answer, 916, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__127)) __PYX_ERR(0, 916, __pyx_L1_error)
+  __pyx_codeobj__130 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__22, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_Fortuna_pyx, __pyx_n_s_get_answer, 931, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__130)) __PYX_ERR(0, 931, __pyx_L1_error)
 
-  /* "Fortuna.pyx":919
+  /* "Fortuna.pyx":934
  *         return input('\n'.join(self.choice_pack)).lower() or self.default
  * 
  *     def __call__(self) -> str:             # <<<<<<<<<<<<<<
  *         """ @return: String. Returns the user's selection. """
  *         selection = self._get_answer()
  */
-  __pyx_tuple__128 = PyTuple_Pack(2, __pyx_n_s_self, __pyx_n_s_selection); if (unlikely(!__pyx_tuple__128)) __PYX_ERR(0, 919, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__128);
-  __Pyx_GIVEREF(__pyx_tuple__128);
-  __pyx_codeobj__129 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__128, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_Fortuna_pyx, __pyx_n_s_call, 919, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__129)) __PYX_ERR(0, 919, __pyx_L1_error)
+  __pyx_tuple__131 = PyTuple_Pack(2, __pyx_n_s_self, __pyx_n_s_selection); if (unlikely(!__pyx_tuple__131)) __PYX_ERR(0, 934, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__131);
+  __Pyx_GIVEREF(__pyx_tuple__131);
+  __pyx_codeobj__132 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__131, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_Fortuna_pyx, __pyx_n_s_call, 934, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__132)) __PYX_ERR(0, 934, __pyx_L1_error)
 
-  /* "Fortuna.pyx":934
+  /* "Fortuna.pyx":949
  * 
  * 
  * def beta_variate(alpha: float, beta: float) -> float:             # <<<<<<<<<<<<<<
  *     return _beta(alpha, beta)
  * 
  */
-  __pyx_tuple__130 = PyTuple_Pack(2, __pyx_n_s_alpha, __pyx_n_s_beta); if (unlikely(!__pyx_tuple__130)) __PYX_ERR(0, 934, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__130);
-  __Pyx_GIVEREF(__pyx_tuple__130);
-  __pyx_codeobj__131 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__130, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_Fortuna_pyx, __pyx_n_s_beta_variate, 934, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__131)) __PYX_ERR(0, 934, __pyx_L1_error)
+  __pyx_tuple__133 = PyTuple_Pack(2, __pyx_n_s_alpha, __pyx_n_s_beta); if (unlikely(!__pyx_tuple__133)) __PYX_ERR(0, 949, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__133);
+  __Pyx_GIVEREF(__pyx_tuple__133);
+  __pyx_codeobj__134 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__133, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_Fortuna_pyx, __pyx_n_s_beta_variate, 949, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__134)) __PYX_ERR(0, 949, __pyx_L1_error)
 
-  /* "Fortuna.pyx":938
+  /* "Fortuna.pyx":953
  * 
  * 
  * def pareto_variate(alpha: float) -> float:             # <<<<<<<<<<<<<<
  *     return _pareto(alpha)
  * 
  */
-  __pyx_tuple__132 = PyTuple_Pack(1, __pyx_n_s_alpha); if (unlikely(!__pyx_tuple__132)) __PYX_ERR(0, 938, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__132);
-  __Pyx_GIVEREF(__pyx_tuple__132);
-  __pyx_codeobj__133 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__132, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_Fortuna_pyx, __pyx_n_s_pareto_variate, 938, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__133)) __PYX_ERR(0, 938, __pyx_L1_error)
+  __pyx_tuple__135 = PyTuple_Pack(1, __pyx_n_s_alpha); if (unlikely(!__pyx_tuple__135)) __PYX_ERR(0, 953, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__135);
+  __Pyx_GIVEREF(__pyx_tuple__135);
+  __pyx_codeobj__136 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__135, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_Fortuna_pyx, __pyx_n_s_pareto_variate, 953, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__136)) __PYX_ERR(0, 953, __pyx_L1_error)
 
-  /* "Fortuna.pyx":942
+  /* "Fortuna.pyx":957
  * 
  * 
  * def vonmises_variate(mu: float, kappa: float) -> float:             # <<<<<<<<<<<<<<
  *     return _vonmises(mu, kappa)
  * 
  */
-  __pyx_tuple__134 = PyTuple_Pack(2, __pyx_n_s_mu, __pyx_n_s_kappa); if (unlikely(!__pyx_tuple__134)) __PYX_ERR(0, 942, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__134);
-  __Pyx_GIVEREF(__pyx_tuple__134);
-  __pyx_codeobj__135 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__134, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_Fortuna_pyx, __pyx_n_s_vonmises_variate, 942, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__135)) __PYX_ERR(0, 942, __pyx_L1_error)
+  __pyx_tuple__137 = PyTuple_Pack(2, __pyx_n_s_mu, __pyx_n_s_kappa); if (unlikely(!__pyx_tuple__137)) __PYX_ERR(0, 957, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__137);
+  __Pyx_GIVEREF(__pyx_tuple__137);
+  __pyx_codeobj__138 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__137, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_Fortuna_pyx, __pyx_n_s_vonmises_variate, 957, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__138)) __PYX_ERR(0, 957, __pyx_L1_error)
 
-  /* "Fortuna.pyx":946
+  /* "Fortuna.pyx":961
  * 
  * 
  * def bernoulli_variate(ratio_of_truth: float) -> bool:             # <<<<<<<<<<<<<<
  *     return _bernoulli(ratio_of_truth) == 1
  * 
  */
-  __pyx_tuple__136 = PyTuple_Pack(1, __pyx_n_s_ratio_of_truth); if (unlikely(!__pyx_tuple__136)) __PYX_ERR(0, 946, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__136);
-  __Pyx_GIVEREF(__pyx_tuple__136);
-  __pyx_codeobj__137 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__136, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_Fortuna_pyx, __pyx_n_s_bernoulli_variate, 946, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__137)) __PYX_ERR(0, 946, __pyx_L1_error)
+  __pyx_tuple__139 = PyTuple_Pack(1, __pyx_n_s_ratio_of_truth); if (unlikely(!__pyx_tuple__139)) __PYX_ERR(0, 961, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__139);
+  __Pyx_GIVEREF(__pyx_tuple__139);
+  __pyx_codeobj__140 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__139, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_Fortuna_pyx, __pyx_n_s_bernoulli_variate, 961, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__140)) __PYX_ERR(0, 961, __pyx_L1_error)
 
-  /* "Fortuna.pyx":950
+  /* "Fortuna.pyx":965
  * 
  * 
  * def binomial_variate(number_of_trials: int, probability: float) -> int:             # <<<<<<<<<<<<<<
  *     return _binomial(number_of_trials, probability)
  * 
  */
-  __pyx_tuple__138 = PyTuple_Pack(2, __pyx_n_s_number_of_trials, __pyx_n_s_probability); if (unlikely(!__pyx_tuple__138)) __PYX_ERR(0, 950, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__138);
-  __Pyx_GIVEREF(__pyx_tuple__138);
-  __pyx_codeobj__139 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__138, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_Fortuna_pyx, __pyx_n_s_binomial_variate, 950, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__139)) __PYX_ERR(0, 950, __pyx_L1_error)
+  __pyx_tuple__141 = PyTuple_Pack(2, __pyx_n_s_number_of_trials, __pyx_n_s_probability); if (unlikely(!__pyx_tuple__141)) __PYX_ERR(0, 965, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__141);
+  __Pyx_GIVEREF(__pyx_tuple__141);
+  __pyx_codeobj__142 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__141, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_Fortuna_pyx, __pyx_n_s_binomial_variate, 965, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__142)) __PYX_ERR(0, 965, __pyx_L1_error)
 
-  /* "Fortuna.pyx":954
+  /* "Fortuna.pyx":969
  * 
  * 
  * def negative_binomial_variate(number_of_trials: int, probability: float) -> int:             # <<<<<<<<<<<<<<
  *     return _neg_binomial(number_of_trials, probability)
  * 
  */
-  __pyx_codeobj__140 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__138, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_Fortuna_pyx, __pyx_n_s_negative_binomial_variate, 954, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__140)) __PYX_ERR(0, 954, __pyx_L1_error)
+  __pyx_codeobj__143 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__141, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_Fortuna_pyx, __pyx_n_s_negative_binomial_variate, 969, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__143)) __PYX_ERR(0, 969, __pyx_L1_error)
 
-  /* "Fortuna.pyx":958
+  /* "Fortuna.pyx":973
  * 
  * 
  * def geometric_variate(probability: float) -> int:             # <<<<<<<<<<<<<<
  *     return _geometric(probability)
  * 
  */
-  __pyx_tuple__141 = PyTuple_Pack(1, __pyx_n_s_probability); if (unlikely(!__pyx_tuple__141)) __PYX_ERR(0, 958, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__141);
-  __Pyx_GIVEREF(__pyx_tuple__141);
-  __pyx_codeobj__142 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__141, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_Fortuna_pyx, __pyx_n_s_geometric_variate, 958, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__142)) __PYX_ERR(0, 958, __pyx_L1_error)
+  __pyx_tuple__144 = PyTuple_Pack(1, __pyx_n_s_probability); if (unlikely(!__pyx_tuple__144)) __PYX_ERR(0, 973, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__144);
+  __Pyx_GIVEREF(__pyx_tuple__144);
+  __pyx_codeobj__145 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__144, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_Fortuna_pyx, __pyx_n_s_geometric_variate, 973, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__145)) __PYX_ERR(0, 973, __pyx_L1_error)
 
-  /* "Fortuna.pyx":962
+  /* "Fortuna.pyx":977
  * 
  * 
  * def poisson_variate(mean: float) -> int:             # <<<<<<<<<<<<<<
  *     return _poisson(mean)
  * 
  */
-  __pyx_tuple__143 = PyTuple_Pack(1, __pyx_n_s_mean); if (unlikely(!__pyx_tuple__143)) __PYX_ERR(0, 962, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__143);
-  __Pyx_GIVEREF(__pyx_tuple__143);
-  __pyx_codeobj__144 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__143, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_Fortuna_pyx, __pyx_n_s_poisson_variate, 962, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__144)) __PYX_ERR(0, 962, __pyx_L1_error)
+  __pyx_tuple__146 = PyTuple_Pack(1, __pyx_n_s_mean); if (unlikely(!__pyx_tuple__146)) __PYX_ERR(0, 977, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__146);
+  __Pyx_GIVEREF(__pyx_tuple__146);
+  __pyx_codeobj__147 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__146, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_Fortuna_pyx, __pyx_n_s_poisson_variate, 977, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__147)) __PYX_ERR(0, 977, __pyx_L1_error)
 
-  /* "Fortuna.pyx":966
+  /* "Fortuna.pyx":981
  * 
  * 
  * def exponential_variate(lambda_rate: float) -> float:             # <<<<<<<<<<<<<<
  *     return _exponential(lambda_rate)
  * 
  */
-  __pyx_tuple__145 = PyTuple_Pack(1, __pyx_n_s_lambda_rate); if (unlikely(!__pyx_tuple__145)) __PYX_ERR(0, 966, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__145);
-  __Pyx_GIVEREF(__pyx_tuple__145);
-  __pyx_codeobj__146 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__145, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_Fortuna_pyx, __pyx_n_s_exponential_variate, 966, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__146)) __PYX_ERR(0, 966, __pyx_L1_error)
+  __pyx_tuple__148 = PyTuple_Pack(1, __pyx_n_s_lambda_rate); if (unlikely(!__pyx_tuple__148)) __PYX_ERR(0, 981, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__148);
+  __Pyx_GIVEREF(__pyx_tuple__148);
+  __pyx_codeobj__149 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__148, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_Fortuna_pyx, __pyx_n_s_exponential_variate, 981, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__149)) __PYX_ERR(0, 981, __pyx_L1_error)
 
-  /* "Fortuna.pyx":970
+  /* "Fortuna.pyx":985
  * 
  * 
  * def gamma_variate(shape: float, scale: float) -> float:             # <<<<<<<<<<<<<<
  *     return _gamma(shape, scale)
  * 
  */
-  __pyx_tuple__147 = PyTuple_Pack(2, __pyx_n_s_shape, __pyx_n_s_scale); if (unlikely(!__pyx_tuple__147)) __PYX_ERR(0, 970, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__147);
-  __Pyx_GIVEREF(__pyx_tuple__147);
-  __pyx_codeobj__148 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__147, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_Fortuna_pyx, __pyx_n_s_gamma_variate, 970, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__148)) __PYX_ERR(0, 970, __pyx_L1_error)
+  __pyx_tuple__150 = PyTuple_Pack(2, __pyx_n_s_shape, __pyx_n_s_scale); if (unlikely(!__pyx_tuple__150)) __PYX_ERR(0, 985, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__150);
+  __Pyx_GIVEREF(__pyx_tuple__150);
+  __pyx_codeobj__151 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__150, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_Fortuna_pyx, __pyx_n_s_gamma_variate, 985, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__151)) __PYX_ERR(0, 985, __pyx_L1_error)
 
-  /* "Fortuna.pyx":974
+  /* "Fortuna.pyx":989
  * 
  * 
  * def weibull_variate(shape: float, scale: float) -> float:             # <<<<<<<<<<<<<<
  *     return _weibull(shape, scale)
  * 
  */
-  __pyx_codeobj__149 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__147, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_Fortuna_pyx, __pyx_n_s_weibull_variate, 974, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__149)) __PYX_ERR(0, 974, __pyx_L1_error)
+  __pyx_codeobj__152 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__150, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_Fortuna_pyx, __pyx_n_s_weibull_variate, 989, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__152)) __PYX_ERR(0, 989, __pyx_L1_error)
 
-  /* "Fortuna.pyx":978
+  /* "Fortuna.pyx":993
  * 
  * 
  * def normal_variate(mean: float, std_dev: float) -> float:             # <<<<<<<<<<<<<<
  *     return _normal(mean, std_dev)
  * 
  */
-  __pyx_tuple__150 = PyTuple_Pack(2, __pyx_n_s_mean, __pyx_n_s_std_dev); if (unlikely(!__pyx_tuple__150)) __PYX_ERR(0, 978, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__150);
-  __Pyx_GIVEREF(__pyx_tuple__150);
-  __pyx_codeobj__151 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__150, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_Fortuna_pyx, __pyx_n_s_normal_variate, 978, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__151)) __PYX_ERR(0, 978, __pyx_L1_error)
+  __pyx_tuple__153 = PyTuple_Pack(2, __pyx_n_s_mean, __pyx_n_s_std_dev); if (unlikely(!__pyx_tuple__153)) __PYX_ERR(0, 993, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__153);
+  __Pyx_GIVEREF(__pyx_tuple__153);
+  __pyx_codeobj__154 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__153, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_Fortuna_pyx, __pyx_n_s_normal_variate, 993, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__154)) __PYX_ERR(0, 993, __pyx_L1_error)
 
-  /* "Fortuna.pyx":982
+  /* "Fortuna.pyx":997
  * 
  * 
  * def log_normal_variate(log_mean: float, log_deviation: float) -> float:             # <<<<<<<<<<<<<<
  *     return _log_normal(log_mean, log_deviation)
  * 
  */
-  __pyx_tuple__152 = PyTuple_Pack(2, __pyx_n_s_log_mean, __pyx_n_s_log_deviation); if (unlikely(!__pyx_tuple__152)) __PYX_ERR(0, 982, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__152);
-  __Pyx_GIVEREF(__pyx_tuple__152);
-  __pyx_codeobj__153 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__152, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_Fortuna_pyx, __pyx_n_s_log_normal_variate, 982, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__153)) __PYX_ERR(0, 982, __pyx_L1_error)
+  __pyx_tuple__155 = PyTuple_Pack(2, __pyx_n_s_log_mean, __pyx_n_s_log_deviation); if (unlikely(!__pyx_tuple__155)) __PYX_ERR(0, 997, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__155);
+  __Pyx_GIVEREF(__pyx_tuple__155);
+  __pyx_codeobj__156 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__155, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_Fortuna_pyx, __pyx_n_s_log_normal_variate, 997, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__156)) __PYX_ERR(0, 997, __pyx_L1_error)
 
-  /* "Fortuna.pyx":986
+  /* "Fortuna.pyx":1001
  * 
  * 
  * def extreme_value_variate(location: float, scale: float) -> float:             # <<<<<<<<<<<<<<
  *     return _extreme_value(location, scale)
  * 
  */
-  __pyx_tuple__154 = PyTuple_Pack(2, __pyx_n_s_location, __pyx_n_s_scale); if (unlikely(!__pyx_tuple__154)) __PYX_ERR(0, 986, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__154);
-  __Pyx_GIVEREF(__pyx_tuple__154);
-  __pyx_codeobj__155 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__154, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_Fortuna_pyx, __pyx_n_s_extreme_value_variate, 986, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__155)) __PYX_ERR(0, 986, __pyx_L1_error)
+  __pyx_tuple__157 = PyTuple_Pack(2, __pyx_n_s_location, __pyx_n_s_scale); if (unlikely(!__pyx_tuple__157)) __PYX_ERR(0, 1001, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__157);
+  __Pyx_GIVEREF(__pyx_tuple__157);
+  __pyx_codeobj__158 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__157, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_Fortuna_pyx, __pyx_n_s_extreme_value_variate, 1001, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__158)) __PYX_ERR(0, 1001, __pyx_L1_error)
 
-  /* "Fortuna.pyx":990
+  /* "Fortuna.pyx":1005
  * 
  * 
  * def chi_squared_variate(degrees_of_freedom: float) -> float:             # <<<<<<<<<<<<<<
  *     return _chi_squared(degrees_of_freedom)
  * 
  */
-  __pyx_tuple__156 = PyTuple_Pack(1, __pyx_n_s_degrees_of_freedom); if (unlikely(!__pyx_tuple__156)) __PYX_ERR(0, 990, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__156);
-  __Pyx_GIVEREF(__pyx_tuple__156);
-  __pyx_codeobj__157 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__156, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_Fortuna_pyx, __pyx_n_s_chi_squared_variate, 990, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__157)) __PYX_ERR(0, 990, __pyx_L1_error)
+  __pyx_tuple__159 = PyTuple_Pack(1, __pyx_n_s_degrees_of_freedom); if (unlikely(!__pyx_tuple__159)) __PYX_ERR(0, 1005, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__159);
+  __Pyx_GIVEREF(__pyx_tuple__159);
+  __pyx_codeobj__160 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__159, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_Fortuna_pyx, __pyx_n_s_chi_squared_variate, 1005, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__160)) __PYX_ERR(0, 1005, __pyx_L1_error)
 
-  /* "Fortuna.pyx":994
+  /* "Fortuna.pyx":1009
  * 
  * 
  * def cauchy_variate(location: float, scale: float) -> float:             # <<<<<<<<<<<<<<
  *     return _cauchy(location, scale)
  * 
  */
-  __pyx_codeobj__158 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__154, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_Fortuna_pyx, __pyx_n_s_cauchy_variate, 994, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__158)) __PYX_ERR(0, 994, __pyx_L1_error)
+  __pyx_codeobj__161 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__157, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_Fortuna_pyx, __pyx_n_s_cauchy_variate, 1009, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__161)) __PYX_ERR(0, 1009, __pyx_L1_error)
 
-  /* "Fortuna.pyx":998
+  /* "Fortuna.pyx":1013
  * 
  * 
  * def fisher_f_variate(degrees_of_freedom_1: float, degrees_of_freedom_2: float) -> float:             # <<<<<<<<<<<<<<
  *     return _fisher_f(degrees_of_freedom_1, degrees_of_freedom_2)
  * 
  */
-  __pyx_tuple__159 = PyTuple_Pack(2, __pyx_n_s_degrees_of_freedom_1, __pyx_n_s_degrees_of_freedom_2); if (unlikely(!__pyx_tuple__159)) __PYX_ERR(0, 998, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__159);
-  __Pyx_GIVEREF(__pyx_tuple__159);
-  __pyx_codeobj__160 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__159, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_Fortuna_pyx, __pyx_n_s_fisher_f_variate, 998, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__160)) __PYX_ERR(0, 998, __pyx_L1_error)
+  __pyx_tuple__162 = PyTuple_Pack(2, __pyx_n_s_degrees_of_freedom_1, __pyx_n_s_degrees_of_freedom_2); if (unlikely(!__pyx_tuple__162)) __PYX_ERR(0, 1013, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__162);
+  __Pyx_GIVEREF(__pyx_tuple__162);
+  __pyx_codeobj__163 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__162, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_Fortuna_pyx, __pyx_n_s_fisher_f_variate, 1013, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__163)) __PYX_ERR(0, 1013, __pyx_L1_error)
 
-  /* "Fortuna.pyx":1002
+  /* "Fortuna.pyx":1017
  * 
  * 
  * def student_t_variate(degrees_of_freedom: float) -> float:             # <<<<<<<<<<<<<<
  *     return _student_t(degrees_of_freedom)
  */
-  __pyx_codeobj__161 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__156, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_Fortuna_pyx, __pyx_n_s_student_t_variate, 1002, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__161)) __PYX_ERR(0, 1002, __pyx_L1_error)
+  __pyx_codeobj__164 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__159, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_Fortuna_pyx, __pyx_n_s_student_t_variate, 1017, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__164)) __PYX_ERR(0, 1017, __pyx_L1_error)
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 /* #### Code section: init_constants ### */
@@ -29419,61 +30021,61 @@
   #endif
   #if !CYTHON_COMPILING_IN_LIMITED_API
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_ptype_7Fortuna___pyx_scope_struct__truffle_shuffle->tp_dictoffset && __pyx_ptype_7Fortuna___pyx_scope_struct__truffle_shuffle->tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_ptype_7Fortuna___pyx_scope_struct__truffle_shuffle->tp_getattro = __Pyx_PyObject_GenericGetAttrNoDict;
   }
   #endif
   #if CYTHON_USE_TYPE_SPECS
-  __pyx_ptype_7Fortuna___pyx_scope_struct_1_genexpr = (PyTypeObject *) __Pyx_PyType_FromModuleAndSpec(__pyx_m, &__pyx_type_7Fortuna___pyx_scope_struct_1_genexpr_spec, NULL); if (unlikely(!__pyx_ptype_7Fortuna___pyx_scope_struct_1_genexpr)) __PYX_ERR(0, 845, __pyx_L1_error)
-  if (__Pyx_fix_up_extension_type_from_spec(&__pyx_type_7Fortuna___pyx_scope_struct_1_genexpr_spec, __pyx_ptype_7Fortuna___pyx_scope_struct_1_genexpr) < 0) __PYX_ERR(0, 845, __pyx_L1_error)
+  __pyx_ptype_7Fortuna___pyx_scope_struct_1_genexpr = (PyTypeObject *) __Pyx_PyType_FromModuleAndSpec(__pyx_m, &__pyx_type_7Fortuna___pyx_scope_struct_1_genexpr_spec, NULL); if (unlikely(!__pyx_ptype_7Fortuna___pyx_scope_struct_1_genexpr)) __PYX_ERR(0, 860, __pyx_L1_error)
+  if (__Pyx_fix_up_extension_type_from_spec(&__pyx_type_7Fortuna___pyx_scope_struct_1_genexpr_spec, __pyx_ptype_7Fortuna___pyx_scope_struct_1_genexpr) < 0) __PYX_ERR(0, 860, __pyx_L1_error)
   #else
   __pyx_ptype_7Fortuna___pyx_scope_struct_1_genexpr = &__pyx_type_7Fortuna___pyx_scope_struct_1_genexpr;
   #endif
   #if !CYTHON_COMPILING_IN_LIMITED_API
   #endif
   #if !CYTHON_USE_TYPE_SPECS
-  if (__Pyx_PyType_Ready(__pyx_ptype_7Fortuna___pyx_scope_struct_1_genexpr) < 0) __PYX_ERR(0, 845, __pyx_L1_error)
+  if (__Pyx_PyType_Ready(__pyx_ptype_7Fortuna___pyx_scope_struct_1_genexpr) < 0) __PYX_ERR(0, 860, __pyx_L1_error)
   #endif
   #if PY_MAJOR_VERSION < 3
   __pyx_ptype_7Fortuna___pyx_scope_struct_1_genexpr->tp_print = 0;
   #endif
   #if !CYTHON_COMPILING_IN_LIMITED_API
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_ptype_7Fortuna___pyx_scope_struct_1_genexpr->tp_dictoffset && __pyx_ptype_7Fortuna___pyx_scope_struct_1_genexpr->tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_ptype_7Fortuna___pyx_scope_struct_1_genexpr->tp_getattro = __Pyx_PyObject_GenericGetAttrNoDict;
   }
   #endif
   #if CYTHON_USE_TYPE_SPECS
-  __pyx_ptype_7Fortuna___pyx_scope_struct_2_genexpr = (PyTypeObject *) __Pyx_PyType_FromModuleAndSpec(__pyx_m, &__pyx_type_7Fortuna___pyx_scope_struct_2_genexpr_spec, NULL); if (unlikely(!__pyx_ptype_7Fortuna___pyx_scope_struct_2_genexpr)) __PYX_ERR(0, 874, __pyx_L1_error)
-  if (__Pyx_fix_up_extension_type_from_spec(&__pyx_type_7Fortuna___pyx_scope_struct_2_genexpr_spec, __pyx_ptype_7Fortuna___pyx_scope_struct_2_genexpr) < 0) __PYX_ERR(0, 874, __pyx_L1_error)
+  __pyx_ptype_7Fortuna___pyx_scope_struct_2_genexpr = (PyTypeObject *) __Pyx_PyType_FromModuleAndSpec(__pyx_m, &__pyx_type_7Fortuna___pyx_scope_struct_2_genexpr_spec, NULL); if (unlikely(!__pyx_ptype_7Fortuna___pyx_scope_struct_2_genexpr)) __PYX_ERR(0, 889, __pyx_L1_error)
+  if (__Pyx_fix_up_extension_type_from_spec(&__pyx_type_7Fortuna___pyx_scope_struct_2_genexpr_spec, __pyx_ptype_7Fortuna___pyx_scope_struct_2_genexpr) < 0) __PYX_ERR(0, 889, __pyx_L1_error)
   #else
   __pyx_ptype_7Fortuna___pyx_scope_struct_2_genexpr = &__pyx_type_7Fortuna___pyx_scope_struct_2_genexpr;
   #endif
   #if !CYTHON_COMPILING_IN_LIMITED_API
   #endif
   #if !CYTHON_USE_TYPE_SPECS
-  if (__Pyx_PyType_Ready(__pyx_ptype_7Fortuna___pyx_scope_struct_2_genexpr) < 0) __PYX_ERR(0, 874, __pyx_L1_error)
+  if (__Pyx_PyType_Ready(__pyx_ptype_7Fortuna___pyx_scope_struct_2_genexpr) < 0) __PYX_ERR(0, 889, __pyx_L1_error)
   #endif
   #if PY_MAJOR_VERSION < 3
   __pyx_ptype_7Fortuna___pyx_scope_struct_2_genexpr->tp_print = 0;
   #endif
   #if !CYTHON_COMPILING_IN_LIMITED_API
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_ptype_7Fortuna___pyx_scope_struct_2_genexpr->tp_dictoffset && __pyx_ptype_7Fortuna___pyx_scope_struct_2_genexpr->tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_ptype_7Fortuna___pyx_scope_struct_2_genexpr->tp_getattro = __Pyx_PyObject_GenericGetAttrNoDict;
   }
   #endif
   #if CYTHON_USE_TYPE_SPECS
-  __pyx_ptype_7Fortuna___pyx_scope_struct_3_genexpr = (PyTypeObject *) __Pyx_PyType_FromModuleAndSpec(__pyx_m, &__pyx_type_7Fortuna___pyx_scope_struct_3_genexpr_spec, NULL); if (unlikely(!__pyx_ptype_7Fortuna___pyx_scope_struct_3_genexpr)) __PYX_ERR(0, 912, __pyx_L1_error)
-  if (__Pyx_fix_up_extension_type_from_spec(&__pyx_type_7Fortuna___pyx_scope_struct_3_genexpr_spec, __pyx_ptype_7Fortuna___pyx_scope_struct_3_genexpr) < 0) __PYX_ERR(0, 912, __pyx_L1_error)
+  __pyx_ptype_7Fortuna___pyx_scope_struct_3_genexpr = (PyTypeObject *) __Pyx_PyType_FromModuleAndSpec(__pyx_m, &__pyx_type_7Fortuna___pyx_scope_struct_3_genexpr_spec, NULL); if (unlikely(!__pyx_ptype_7Fortuna___pyx_scope_struct_3_genexpr)) __PYX_ERR(0, 927, __pyx_L1_error)
+  if (__Pyx_fix_up_extension_type_from_spec(&__pyx_type_7Fortuna___pyx_scope_struct_3_genexpr_spec, __pyx_ptype_7Fortuna___pyx_scope_struct_3_genexpr) < 0) __PYX_ERR(0, 927, __pyx_L1_error)
   #else
   __pyx_ptype_7Fortuna___pyx_scope_struct_3_genexpr = &__pyx_type_7Fortuna___pyx_scope_struct_3_genexpr;
   #endif
   #if !CYTHON_COMPILING_IN_LIMITED_API
   #endif
   #if !CYTHON_USE_TYPE_SPECS
-  if (__Pyx_PyType_Ready(__pyx_ptype_7Fortuna___pyx_scope_struct_3_genexpr) < 0) __PYX_ERR(0, 912, __pyx_L1_error)
+  if (__Pyx_PyType_Ready(__pyx_ptype_7Fortuna___pyx_scope_struct_3_genexpr) < 0) __PYX_ERR(0, 927, __pyx_L1_error)
   #endif
   #if PY_MAJOR_VERSION < 3
   __pyx_ptype_7Fortuna___pyx_scope_struct_3_genexpr->tp_print = 0;
   #endif
   #if !CYTHON_COMPILING_IN_LIMITED_API
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_ptype_7Fortuna___pyx_scope_struct_3_genexpr->tp_dictoffset && __pyx_ptype_7Fortuna___pyx_scope_struct_3_genexpr->tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_ptype_7Fortuna___pyx_scope_struct_3_genexpr->tp_getattro = __Pyx_PyObject_GenericGetAttrNoDict;
@@ -29814,15 +30416,15 @@
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
   /* "Fortuna.pyx":4
  * #distutils: language = c++
  * from collections import deque
  * from itertools import cycle             # <<<<<<<<<<<<<<
  * from math import sqrt
- * from typing import Callable, Iterable, Dict
+ * from typing import Callable, Iterable, Dict, Iterator
  */
   __pyx_t_3 = PyList_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_INCREF(__pyx_n_s_cycle);
   __Pyx_GIVEREF(__pyx_n_s_cycle);
   if (__Pyx_PyList_SET_ITEM(__pyx_t_3, 0, __pyx_n_s_cycle)) __PYX_ERR(0, 4, __pyx_L1_error);
   __pyx_t_2 = __Pyx_Import(__pyx_n_s_itertools, __pyx_t_3, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 4, __pyx_L1_error)
@@ -29834,15 +30436,15 @@
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "Fortuna.pyx":5
  * from collections import deque
  * from itertools import cycle
  * from math import sqrt             # <<<<<<<<<<<<<<
- * from typing import Callable, Iterable, Dict
+ * from typing import Callable, Iterable, Dict, Iterator
  * 
  */
   __pyx_t_2 = PyList_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 5, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_INCREF(__pyx_n_s_sqrt);
   __Pyx_GIVEREF(__pyx_n_s_sqrt);
   if (__Pyx_PyList_SET_ITEM(__pyx_t_2, 0, __pyx_n_s_sqrt)) __PYX_ERR(0, 5, __pyx_L1_error);
@@ -29854,29 +30456,32 @@
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_sqrt, __pyx_t_2) < 0) __PYX_ERR(0, 5, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
   /* "Fortuna.pyx":6
  * from itertools import cycle
  * from math import sqrt
- * from typing import Callable, Iterable, Dict             # <<<<<<<<<<<<<<
+ * from typing import Callable, Iterable, Dict, Iterator             # <<<<<<<<<<<<<<
  * 
  * version = "5.5.1"
  */
-  __pyx_t_3 = PyList_New(3); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 6, __pyx_L1_error)
+  __pyx_t_3 = PyList_New(4); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 6, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_INCREF(__pyx_n_s_Callable);
   __Pyx_GIVEREF(__pyx_n_s_Callable);
   if (__Pyx_PyList_SET_ITEM(__pyx_t_3, 0, __pyx_n_s_Callable)) __PYX_ERR(0, 6, __pyx_L1_error);
   __Pyx_INCREF(__pyx_n_s_Iterable);
   __Pyx_GIVEREF(__pyx_n_s_Iterable);
   if (__Pyx_PyList_SET_ITEM(__pyx_t_3, 1, __pyx_n_s_Iterable)) __PYX_ERR(0, 6, __pyx_L1_error);
   __Pyx_INCREF(__pyx_n_s_Dict);
   __Pyx_GIVEREF(__pyx_n_s_Dict);
   if (__Pyx_PyList_SET_ITEM(__pyx_t_3, 2, __pyx_n_s_Dict)) __PYX_ERR(0, 6, __pyx_L1_error);
+  __Pyx_INCREF(__pyx_n_s_Iterator);
+  __Pyx_GIVEREF(__pyx_n_s_Iterator);
+  if (__Pyx_PyList_SET_ITEM(__pyx_t_3, 3, __pyx_n_s_Iterator)) __PYX_ERR(0, 6, __pyx_L1_error);
   __pyx_t_2 = __Pyx_Import(__pyx_n_s_typing, __pyx_t_3, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 6, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_t_3 = __Pyx_ImportFrom(__pyx_t_2, __pyx_n_s_Callable); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 6, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_Callable, __pyx_t_3) < 0) __PYX_ERR(0, 6, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
@@ -29884,18 +30489,22 @@
   __Pyx_GOTREF(__pyx_t_3);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_Iterable, __pyx_t_3) < 0) __PYX_ERR(0, 6, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_t_3 = __Pyx_ImportFrom(__pyx_t_2, __pyx_n_s_Dict); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 6, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_Dict, __pyx_t_3) < 0) __PYX_ERR(0, 6, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  __pyx_t_3 = __Pyx_ImportFrom(__pyx_t_2, __pyx_n_s_Iterator); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 6, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_Iterator, __pyx_t_3) < 0) __PYX_ERR(0, 6, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "Fortuna.pyx":8
- * from typing import Callable, Iterable, Dict
+ * from typing import Callable, Iterable, Dict, Iterator
  * 
  * version = "5.5.1"             # <<<<<<<<<<<<<<
  * 
  * cdef extern from "Storm.hpp":
  */
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_version, __pyx_kp_u_5_5_1) < 0) __PYX_ERR(0, 8, __pyx_L1_error)
 
@@ -31128,1009 +31737,1072 @@
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_RandomValue, __pyx_t_2) < 0) __PYX_ERR(0, 523, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
   /* "Fortuna.pyx":552
  * 
  * 
+ * class TruffleShuffle2:             # <<<<<<<<<<<<<<
+ *     __slots__ = ("flat", "data", "size", "pivot", "index")
+ * 
+ */
+  __pyx_t_3 = __Pyx_Py3MetaclassPrepare((PyObject *) NULL, __pyx_empty_tuple, __pyx_n_s_TruffleShuffle2, __pyx_n_s_TruffleShuffle2, (PyObject *) NULL, __pyx_n_s_Fortuna, (PyObject *) NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 552, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+
+  /* "Fortuna.pyx":553
+ * 
+ * class TruffleShuffle2:
+ *     __slots__ = ("flat", "data", "size", "pivot", "index")             # <<<<<<<<<<<<<<
+ * 
+ *     def __init__(self, collection: Iterable, flat: bool = True):
+ */
+  if (__Pyx_SetNameInClass(__pyx_t_3, __pyx_n_s_slots, __pyx_tuple__85) < 0) __PYX_ERR(0, 553, __pyx_L1_error)
+
+  /* "Fortuna.pyx":555
+ *     __slots__ = ("flat", "data", "size", "pivot", "index")
+ * 
+ *     def __init__(self, collection: Iterable, flat: bool = True):             # <<<<<<<<<<<<<<
+ *         self.flat = flat
+ *         self.data = list(collection) if isinstance(collection, Iterator) else collection
+ */
+  __pyx_t_2 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 555, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_collection, __pyx_n_s_Iterable) < 0) __PYX_ERR(0, 555, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_flat, __pyx_n_s_bool) < 0) __PYX_ERR(0, 555, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_7Fortuna_15TruffleShuffle2_1__init__, 0, __pyx_n_s_TruffleShuffle2___init, NULL, __pyx_n_s_Fortuna, __pyx_d, ((PyObject *)__pyx_codeobj__87)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 555, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_4, __pyx_tuple__88);
+  __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_4, __pyx_t_2);
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  if (__Pyx_SetNameInClass(__pyx_t_3, __pyx_n_s_init, __pyx_t_4) < 0) __PYX_ERR(0, 555, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+
+  /* "Fortuna.pyx":562
+ *         self.index = _random_index(self.size)
+ * 
+ *     def __call__(self, *args, **kwargs):             # <<<<<<<<<<<<<<
+ *         self.index = (self.index + 1 + _front_poisson(self.pivot)) % self.size
+ *         return flatten(self.data[self.index], *args, flat=self.flat, **kwargs)
+ */
+  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_7Fortuna_15TruffleShuffle2_3__call__, 0, __pyx_n_s_TruffleShuffle2___call, NULL, __pyx_n_s_Fortuna, __pyx_d, ((PyObject *)__pyx_codeobj__89)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 562, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  if (__Pyx_SetNameInClass(__pyx_t_3, __pyx_n_s_call, __pyx_t_4) < 0) __PYX_ERR(0, 562, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+
+  /* "Fortuna.pyx":552
+ * 
+ * 
+ * class TruffleShuffle2:             # <<<<<<<<<<<<<<
+ *     __slots__ = ("flat", "data", "size", "pivot", "index")
+ * 
+ */
+  __pyx_t_4 = __Pyx_Py3ClassCreate(((PyObject*)&PyType_Type), __pyx_n_s_TruffleShuffle2, __pyx_empty_tuple, __pyx_t_3, NULL, 0, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 552, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_TruffleShuffle2, __pyx_t_4) < 0) __PYX_ERR(0, 552, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+
+  /* "Fortuna.pyx":567
+ * 
+ * 
  * class TruffleShuffle:             # <<<<<<<<<<<<<<
  *     """ Truffle Shuffle
  *     Produces random values from a collection with a Wide Uniform Distribution.
  */
-  __pyx_t_3 = __Pyx_Py3MetaclassPrepare((PyObject *) NULL, __pyx_empty_tuple, __pyx_n_s_TruffleShuffle, __pyx_n_s_TruffleShuffle, (PyObject *) NULL, __pyx_n_s_Fortuna, __pyx_kp_s_Truffle_Shuffle_Produces_random); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 552, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_Py3MetaclassPrepare((PyObject *) NULL, __pyx_empty_tuple, __pyx_n_s_TruffleShuffle, __pyx_n_s_TruffleShuffle, (PyObject *) NULL, __pyx_n_s_Fortuna, __pyx_kp_s_Truffle_Shuffle_Produces_random); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 567, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
 
-  /* "Fortuna.pyx":581
+  /* "Fortuna.pyx":596
  *     Please refer to https://pypi.org/project/Fortuna/ for full documentation.
  *     """
  *     __slots__ = ("flat", "data", "rotate_size")             # <<<<<<<<<<<<<<
  * 
  *     def __init__(self, collection: Iterable, flat: bool = True):
  */
-  if (__Pyx_SetNameInClass(__pyx_t_3, __pyx_n_s_slots, __pyx_tuple__85) < 0) __PYX_ERR(0, 581, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_3, __pyx_n_s_slots, __pyx_tuple__90) < 0) __PYX_ERR(0, 596, __pyx_L1_error)
 
-  /* "Fortuna.pyx":583
+  /* "Fortuna.pyx":598
  *     __slots__ = ("flat", "data", "rotate_size")
  * 
  *     def __init__(self, collection: Iterable, flat: bool = True):             # <<<<<<<<<<<<<<
  *         self.flat = flat
  *         data = list(collection)
  */
-  __pyx_t_2 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 583, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_collection, __pyx_n_s_Iterable) < 0) __PYX_ERR(0, 583, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_flat, __pyx_n_s_bool) < 0) __PYX_ERR(0, 583, __pyx_L1_error)
-  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_7Fortuna_14TruffleShuffle_1__init__, 0, __pyx_n_s_TruffleShuffle___init, NULL, __pyx_n_s_Fortuna, __pyx_d, ((PyObject *)__pyx_codeobj__87)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 583, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 598, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_4, __pyx_tuple__88);
-  __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_4, __pyx_t_2);
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (__Pyx_SetNameInClass(__pyx_t_3, __pyx_n_s_init, __pyx_t_4) < 0) __PYX_ERR(0, 583, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_collection, __pyx_n_s_Iterable) < 0) __PYX_ERR(0, 598, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_flat, __pyx_n_s_bool) < 0) __PYX_ERR(0, 598, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_7Fortuna_14TruffleShuffle_1__init__, 0, __pyx_n_s_TruffleShuffle___init, NULL, __pyx_n_s_Fortuna, __pyx_d, ((PyObject *)__pyx_codeobj__92)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 598, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_2, __pyx_tuple__88);
+  __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_2, __pyx_t_4);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  if (__Pyx_SetNameInClass(__pyx_t_3, __pyx_n_s_init, __pyx_t_2) < 0) __PYX_ERR(0, 598, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "Fortuna.pyx":590
+  /* "Fortuna.pyx":605
  *         self.rotate_size = int(sqrt(len(self.data)))
  * 
  *     def __call__(self, *args, **kwargs):             # <<<<<<<<<<<<<<
  *         self.data.rotate(1 + _front_poisson(self.rotate_size))
  *         return flatten(self.data[-1], *args, flat=self.flat, **kwargs)
  */
-  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_7Fortuna_14TruffleShuffle_3__call__, 0, __pyx_n_s_TruffleShuffle___call, NULL, __pyx_n_s_Fortuna, __pyx_d, ((PyObject *)__pyx_codeobj__89)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 590, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_4);
-  if (__Pyx_SetNameInClass(__pyx_t_3, __pyx_n_s_call, __pyx_t_4) < 0) __PYX_ERR(0, 590, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_7Fortuna_14TruffleShuffle_3__call__, 0, __pyx_n_s_TruffleShuffle___call, NULL, __pyx_n_s_Fortuna, __pyx_d, ((PyObject *)__pyx_codeobj__93)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 605, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  if (__Pyx_SetNameInClass(__pyx_t_3, __pyx_n_s_call, __pyx_t_2) < 0) __PYX_ERR(0, 605, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "Fortuna.pyx":552
+  /* "Fortuna.pyx":567
  * 
  * 
  * class TruffleShuffle:             # <<<<<<<<<<<<<<
  *     """ Truffle Shuffle
  *     Produces random values from a collection with a Wide Uniform Distribution.
  */
-  __pyx_t_4 = __Pyx_Py3ClassCreate(((PyObject*)&PyType_Type), __pyx_n_s_TruffleShuffle, __pyx_empty_tuple, __pyx_t_3, NULL, 0, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 552, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_4);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_TruffleShuffle, __pyx_t_4) < 0) __PYX_ERR(0, 552, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  __pyx_t_2 = __Pyx_Py3ClassCreate(((PyObject*)&PyType_Type), __pyx_n_s_TruffleShuffle, __pyx_empty_tuple, __pyx_t_3, NULL, 0, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 567, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_TruffleShuffle, __pyx_t_2) < 0) __PYX_ERR(0, 567, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "Fortuna.pyx":595
+  /* "Fortuna.pyx":610
  * 
  * 
  * class QuantumMonty:             # <<<<<<<<<<<<<<
  *     """ Quantum Monty
  *     @param collection : Collection of Values.
  */
-  __pyx_t_3 = __Pyx_Py3MetaclassPrepare((PyObject *) NULL, __pyx_empty_tuple, __pyx_n_s_QuantumMonty, __pyx_n_s_QuantumMonty, (PyObject *) NULL, __pyx_n_s_Fortuna, __pyx_kp_s_Quantum_Monty_param_collection); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 595, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_Py3MetaclassPrepare((PyObject *) NULL, __pyx_empty_tuple, __pyx_n_s_QuantumMonty, __pyx_n_s_QuantumMonty, (PyObject *) NULL, __pyx_n_s_Fortuna, __pyx_kp_s_Quantum_Monty_param_collection); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 610, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
 
-  /* "Fortuna.pyx":608
+  /* "Fortuna.pyx":623
  *     Please refer to https://pypi.org/project/Fortuna/ for full documentation.
  *     """
  *     __slots__ = ("flat", "size", "data", "truffle_shuffle", "cycles")             # <<<<<<<<<<<<<<
  * 
  *     def __init__(self, collection: Iterable, flat: bool = True):
  */
-  if (__Pyx_SetNameInClass(__pyx_t_3, __pyx_n_s_slots, __pyx_tuple__90) < 0) __PYX_ERR(0, 608, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_3, __pyx_n_s_slots, __pyx_tuple__94) < 0) __PYX_ERR(0, 623, __pyx_L1_error)
 
-  /* "Fortuna.pyx":610
+  /* "Fortuna.pyx":625
  *     __slots__ = ("flat", "size", "data", "truffle_shuffle", "cycles")
  * 
  *     def __init__(self, collection: Iterable, flat: bool = True):             # <<<<<<<<<<<<<<
  *         self.flat = flat
  *         self.data = tuple(collection)
  */
-  __pyx_t_4 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 610, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_4);
-  if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_collection, __pyx_n_s_Iterable) < 0) __PYX_ERR(0, 610, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_flat, __pyx_n_s_bool) < 0) __PYX_ERR(0, 610, __pyx_L1_error)
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_7Fortuna_12QuantumMonty_1__init__, 0, __pyx_n_s_QuantumMonty___init, NULL, __pyx_n_s_Fortuna, __pyx_d, ((PyObject *)__pyx_codeobj__92)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 610, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 625, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_2, __pyx_tuple__88);
-  __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_2, __pyx_t_4);
-  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (__Pyx_SetNameInClass(__pyx_t_3, __pyx_n_s_init, __pyx_t_2) < 0) __PYX_ERR(0, 610, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_collection, __pyx_n_s_Iterable) < 0) __PYX_ERR(0, 625, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_flat, __pyx_n_s_bool) < 0) __PYX_ERR(0, 625, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_7Fortuna_12QuantumMonty_1__init__, 0, __pyx_n_s_QuantumMonty___init, NULL, __pyx_n_s_Fortuna, __pyx_d, ((PyObject *)__pyx_codeobj__95)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 625, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_4, __pyx_tuple__88);
+  __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_4, __pyx_t_2);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  if (__Pyx_SetNameInClass(__pyx_t_3, __pyx_n_s_init, __pyx_t_4) < 0) __PYX_ERR(0, 625, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "Fortuna.pyx":618
+  /* "Fortuna.pyx":633
  *         self.truffle_shuffle = TruffleShuffle(self.data, flat)
  * 
  *     def __call__(self, *args, **kwargs):             # <<<<<<<<<<<<<<
  *         return self.quantum_monty(*args, **kwargs)
  * 
  */
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_7Fortuna_12QuantumMonty_3__call__, 0, __pyx_n_s_QuantumMonty___call, NULL, __pyx_n_s_Fortuna, __pyx_d, ((PyObject *)__pyx_codeobj__93)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 618, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  if (__Pyx_SetNameInClass(__pyx_t_3, __pyx_n_s_call, __pyx_t_2) < 0) __PYX_ERR(0, 618, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_7Fortuna_12QuantumMonty_3__call__, 0, __pyx_n_s_QuantumMonty___call, NULL, __pyx_n_s_Fortuna, __pyx_d, ((PyObject *)__pyx_codeobj__96)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 633, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  if (__Pyx_SetNameInClass(__pyx_t_3, __pyx_n_s_call, __pyx_t_4) < 0) __PYX_ERR(0, 633, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "Fortuna.pyx":621
+  /* "Fortuna.pyx":636
  *         return self.quantum_monty(*args, **kwargs)
  * 
  *     def dispatch(self, monty: str) -> Callable:             # <<<<<<<<<<<<<<
  *         """ For dispatch automation.
  *         In general, prefer to use the methods directly when possible. """
  */
-  __pyx_t_2 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 621, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_monty, __pyx_n_s_str) < 0) __PYX_ERR(0, 621, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_return, __pyx_n_s_Callable) < 0) __PYX_ERR(0, 621, __pyx_L1_error)
-  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_7Fortuna_12QuantumMonty_5dispatch, 0, __pyx_n_s_QuantumMonty_dispatch, NULL, __pyx_n_s_Fortuna, __pyx_d, ((PyObject *)__pyx_codeobj__95)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 621, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 636, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_4, __pyx_t_2);
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (__Pyx_SetNameInClass(__pyx_t_3, __pyx_n_s_dispatch, __pyx_t_4) < 0) __PYX_ERR(0, 621, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_monty, __pyx_n_s_str) < 0) __PYX_ERR(0, 636, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_return, __pyx_n_s_Callable) < 0) __PYX_ERR(0, 636, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_7Fortuna_12QuantumMonty_5dispatch, 0, __pyx_n_s_QuantumMonty_dispatch, NULL, __pyx_n_s_Fortuna, __pyx_d, ((PyObject *)__pyx_codeobj__98)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 636, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_2, __pyx_t_4);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  if (__Pyx_SetNameInClass(__pyx_t_3, __pyx_n_s_dispatch, __pyx_t_2) < 0) __PYX_ERR(0, 636, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "Fortuna.pyx":643
+  /* "Fortuna.pyx":658
  *         }[monty]
  * 
  *     def flat_uniform(self, *args, **kwargs):             # <<<<<<<<<<<<<<
  *         return flatten(
  *             self.data[_random_index(self.size)], *args, flat=self.flat, **kwargs
  */
-  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_7Fortuna_12QuantumMonty_7flat_uniform, 0, __pyx_n_s_QuantumMonty_flat_uniform, NULL, __pyx_n_s_Fortuna, __pyx_d, ((PyObject *)__pyx_codeobj__96)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 643, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_4);
-  if (__Pyx_SetNameInClass(__pyx_t_3, __pyx_n_s_flat_uniform, __pyx_t_4) < 0) __PYX_ERR(0, 643, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_7Fortuna_12QuantumMonty_7flat_uniform, 0, __pyx_n_s_QuantumMonty_flat_uniform, NULL, __pyx_n_s_Fortuna, __pyx_d, ((PyObject *)__pyx_codeobj__99)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 658, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  if (__Pyx_SetNameInClass(__pyx_t_3, __pyx_n_s_flat_uniform, __pyx_t_2) < 0) __PYX_ERR(0, 658, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "Fortuna.pyx":648
+  /* "Fortuna.pyx":663
  *         )
  * 
  *     def cycle(self, *args, **kwargs):             # <<<<<<<<<<<<<<
  *         return flatten(
  *             next(self.cycles), *args, flat=self.flat, **kwargs
  */
-  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_7Fortuna_12QuantumMonty_9cycle, 0, __pyx_n_s_QuantumMonty_cycle, NULL, __pyx_n_s_Fortuna, __pyx_d, ((PyObject *)__pyx_codeobj__97)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 648, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_4);
-  if (__Pyx_SetNameInClass(__pyx_t_3, __pyx_n_s_cycle, __pyx_t_4) < 0) __PYX_ERR(0, 648, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_7Fortuna_12QuantumMonty_9cycle, 0, __pyx_n_s_QuantumMonty_cycle, NULL, __pyx_n_s_Fortuna, __pyx_d, ((PyObject *)__pyx_codeobj__100)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 663, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  if (__Pyx_SetNameInClass(__pyx_t_3, __pyx_n_s_cycle, __pyx_t_2) < 0) __PYX_ERR(0, 663, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "Fortuna.pyx":653
+  /* "Fortuna.pyx":668
  *         )
  * 
  *     def front_linear(self, *args, **kwargs):             # <<<<<<<<<<<<<<
  *         return flatten(
  *             self.data[_front_linear(self.size)], *args, flat=self.flat, **kwargs
  */
-  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_7Fortuna_12QuantumMonty_11front_linear, 0, __pyx_n_s_QuantumMonty_front_linear, NULL, __pyx_n_s_Fortuna, __pyx_d, ((PyObject *)__pyx_codeobj__98)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 653, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_4);
-  if (__Pyx_SetNameInClass(__pyx_t_3, __pyx_n_s_front_linear, __pyx_t_4) < 0) __PYX_ERR(0, 653, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_7Fortuna_12QuantumMonty_11front_linear, 0, __pyx_n_s_QuantumMonty_front_linear, NULL, __pyx_n_s_Fortuna, __pyx_d, ((PyObject *)__pyx_codeobj__101)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 668, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  if (__Pyx_SetNameInClass(__pyx_t_3, __pyx_n_s_front_linear, __pyx_t_2) < 0) __PYX_ERR(0, 668, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "Fortuna.pyx":658
+  /* "Fortuna.pyx":673
  *         )
  * 
  *     def middle_linear(self, *args, **kwargs):             # <<<<<<<<<<<<<<
  *         return flatten(
  *             self.data[_middle_linear(self.size)], *args, flat=self.flat, **kwargs
  */
-  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_7Fortuna_12QuantumMonty_13middle_linear, 0, __pyx_n_s_QuantumMonty_middle_linear, NULL, __pyx_n_s_Fortuna, __pyx_d, ((PyObject *)__pyx_codeobj__99)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 658, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_4);
-  if (__Pyx_SetNameInClass(__pyx_t_3, __pyx_n_s_middle_linear, __pyx_t_4) < 0) __PYX_ERR(0, 658, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_7Fortuna_12QuantumMonty_13middle_linear, 0, __pyx_n_s_QuantumMonty_middle_linear, NULL, __pyx_n_s_Fortuna, __pyx_d, ((PyObject *)__pyx_codeobj__102)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 673, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  if (__Pyx_SetNameInClass(__pyx_t_3, __pyx_n_s_middle_linear, __pyx_t_2) < 0) __PYX_ERR(0, 673, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "Fortuna.pyx":663
+  /* "Fortuna.pyx":678
  *         )
  * 
  *     def back_linear(self, *args, **kwargs):             # <<<<<<<<<<<<<<
  *         return flatten(
  *             self.data[_back_linear(self.size)], *args, flat=self.flat, **kwargs
  */
-  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_7Fortuna_12QuantumMonty_15back_linear, 0, __pyx_n_s_QuantumMonty_back_linear, NULL, __pyx_n_s_Fortuna, __pyx_d, ((PyObject *)__pyx_codeobj__100)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 663, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_4);
-  if (__Pyx_SetNameInClass(__pyx_t_3, __pyx_n_s_back_linear, __pyx_t_4) < 0) __PYX_ERR(0, 663, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_7Fortuna_12QuantumMonty_15back_linear, 0, __pyx_n_s_QuantumMonty_back_linear, NULL, __pyx_n_s_Fortuna, __pyx_d, ((PyObject *)__pyx_codeobj__103)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 678, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  if (__Pyx_SetNameInClass(__pyx_t_3, __pyx_n_s_back_linear, __pyx_t_2) < 0) __PYX_ERR(0, 678, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "Fortuna.pyx":668
+  /* "Fortuna.pyx":683
  *         )
  * 
  *     def quantum_linear(self, *args, **kwargs):             # <<<<<<<<<<<<<<
  *         return flatten(
  *             self.data[_quantum_linear(self.size)], *args, flat=self.flat, **kwargs
  */
-  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_7Fortuna_12QuantumMonty_17quantum_linear, 0, __pyx_n_s_QuantumMonty_quantum_linear, NULL, __pyx_n_s_Fortuna, __pyx_d, ((PyObject *)__pyx_codeobj__101)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 668, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_4);
-  if (__Pyx_SetNameInClass(__pyx_t_3, __pyx_n_s_quantum_linear, __pyx_t_4) < 0) __PYX_ERR(0, 668, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_7Fortuna_12QuantumMonty_17quantum_linear, 0, __pyx_n_s_QuantumMonty_quantum_linear, NULL, __pyx_n_s_Fortuna, __pyx_d, ((PyObject *)__pyx_codeobj__104)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 683, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  if (__Pyx_SetNameInClass(__pyx_t_3, __pyx_n_s_quantum_linear, __pyx_t_2) < 0) __PYX_ERR(0, 683, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "Fortuna.pyx":673
+  /* "Fortuna.pyx":688
  *         )
  * 
  *     def front_gauss(self, *args, **kwargs):             # <<<<<<<<<<<<<<
  *         return flatten(
  *             self.data[_front_gauss(self.size)], *args, flat=self.flat, **kwargs)
  */
-  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_7Fortuna_12QuantumMonty_19front_gauss, 0, __pyx_n_s_QuantumMonty_front_gauss, NULL, __pyx_n_s_Fortuna, __pyx_d, ((PyObject *)__pyx_codeobj__102)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 673, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_4);
-  if (__Pyx_SetNameInClass(__pyx_t_3, __pyx_n_s_front_gauss, __pyx_t_4) < 0) __PYX_ERR(0, 673, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_7Fortuna_12QuantumMonty_19front_gauss, 0, __pyx_n_s_QuantumMonty_front_gauss, NULL, __pyx_n_s_Fortuna, __pyx_d, ((PyObject *)__pyx_codeobj__105)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 688, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  if (__Pyx_SetNameInClass(__pyx_t_3, __pyx_n_s_front_gauss, __pyx_t_2) < 0) __PYX_ERR(0, 688, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "Fortuna.pyx":677
+  /* "Fortuna.pyx":692
  *             self.data[_front_gauss(self.size)], *args, flat=self.flat, **kwargs)
  * 
  *     def middle_gauss(self, *args, **kwargs):             # <<<<<<<<<<<<<<
  *         return flatten(
  *             self.data[_middle_gauss(self.size)], *args, flat=self.flat, **kwargs
  */
-  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_7Fortuna_12QuantumMonty_21middle_gauss, 0, __pyx_n_s_QuantumMonty_middle_gauss, NULL, __pyx_n_s_Fortuna, __pyx_d, ((PyObject *)__pyx_codeobj__103)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 677, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_4);
-  if (__Pyx_SetNameInClass(__pyx_t_3, __pyx_n_s_middle_gauss, __pyx_t_4) < 0) __PYX_ERR(0, 677, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_7Fortuna_12QuantumMonty_21middle_gauss, 0, __pyx_n_s_QuantumMonty_middle_gauss, NULL, __pyx_n_s_Fortuna, __pyx_d, ((PyObject *)__pyx_codeobj__106)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 692, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  if (__Pyx_SetNameInClass(__pyx_t_3, __pyx_n_s_middle_gauss, __pyx_t_2) < 0) __PYX_ERR(0, 692, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "Fortuna.pyx":682
+  /* "Fortuna.pyx":697
  *         )
  * 
  *     def back_gauss(self, *args, **kwargs):             # <<<<<<<<<<<<<<
  *         return flatten(
  *             self.data[_back_gauss(self.size)], *args, flat=self.flat, **kwargs
  */
-  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_7Fortuna_12QuantumMonty_23back_gauss, 0, __pyx_n_s_QuantumMonty_back_gauss, NULL, __pyx_n_s_Fortuna, __pyx_d, ((PyObject *)__pyx_codeobj__104)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 682, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_4);
-  if (__Pyx_SetNameInClass(__pyx_t_3, __pyx_n_s_back_gauss, __pyx_t_4) < 0) __PYX_ERR(0, 682, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_7Fortuna_12QuantumMonty_23back_gauss, 0, __pyx_n_s_QuantumMonty_back_gauss, NULL, __pyx_n_s_Fortuna, __pyx_d, ((PyObject *)__pyx_codeobj__107)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 697, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  if (__Pyx_SetNameInClass(__pyx_t_3, __pyx_n_s_back_gauss, __pyx_t_2) < 0) __PYX_ERR(0, 697, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "Fortuna.pyx":687
+  /* "Fortuna.pyx":702
  *         )
  * 
  *     def quantum_gauss(self, *args, **kwargs):             # <<<<<<<<<<<<<<
  *         return flatten(
  *             self.data[_quantum_gauss(self.size)], *args, flat=self.flat, **kwargs
  */
-  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_7Fortuna_12QuantumMonty_25quantum_gauss, 0, __pyx_n_s_QuantumMonty_quantum_gauss, NULL, __pyx_n_s_Fortuna, __pyx_d, ((PyObject *)__pyx_codeobj__105)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 687, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_4);
-  if (__Pyx_SetNameInClass(__pyx_t_3, __pyx_n_s_quantum_gauss, __pyx_t_4) < 0) __PYX_ERR(0, 687, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_7Fortuna_12QuantumMonty_25quantum_gauss, 0, __pyx_n_s_QuantumMonty_quantum_gauss, NULL, __pyx_n_s_Fortuna, __pyx_d, ((PyObject *)__pyx_codeobj__108)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 702, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  if (__Pyx_SetNameInClass(__pyx_t_3, __pyx_n_s_quantum_gauss, __pyx_t_2) < 0) __PYX_ERR(0, 702, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "Fortuna.pyx":692
+  /* "Fortuna.pyx":707
  *         )
  * 
  *     def front_poisson(self, *args, **kwargs):             # <<<<<<<<<<<<<<
  *         return flatten(
  *             self.data[_front_poisson(self.size)], *args, flat=self.flat, **kwargs
  */
-  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_7Fortuna_12QuantumMonty_27front_poisson, 0, __pyx_n_s_QuantumMonty_front_poisson, NULL, __pyx_n_s_Fortuna, __pyx_d, ((PyObject *)__pyx_codeobj__106)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 692, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_4);
-  if (__Pyx_SetNameInClass(__pyx_t_3, __pyx_n_s_front_poisson, __pyx_t_4) < 0) __PYX_ERR(0, 692, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_7Fortuna_12QuantumMonty_27front_poisson, 0, __pyx_n_s_QuantumMonty_front_poisson, NULL, __pyx_n_s_Fortuna, __pyx_d, ((PyObject *)__pyx_codeobj__109)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 707, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  if (__Pyx_SetNameInClass(__pyx_t_3, __pyx_n_s_front_poisson, __pyx_t_2) < 0) __PYX_ERR(0, 707, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "Fortuna.pyx":697
+  /* "Fortuna.pyx":712
  *         )
  * 
  *     def middle_poisson(self, *args, **kwargs):             # <<<<<<<<<<<<<<
  *         return flatten(
  *             self.data[_middle_poisson(self.size)], *args, flat=self.flat, **kwargs
  */
-  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_7Fortuna_12QuantumMonty_29middle_poisson, 0, __pyx_n_s_QuantumMonty_middle_poisson, NULL, __pyx_n_s_Fortuna, __pyx_d, ((PyObject *)__pyx_codeobj__107)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 697, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_4);
-  if (__Pyx_SetNameInClass(__pyx_t_3, __pyx_n_s_middle_poisson, __pyx_t_4) < 0) __PYX_ERR(0, 697, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_7Fortuna_12QuantumMonty_29middle_poisson, 0, __pyx_n_s_QuantumMonty_middle_poisson, NULL, __pyx_n_s_Fortuna, __pyx_d, ((PyObject *)__pyx_codeobj__110)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 712, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  if (__Pyx_SetNameInClass(__pyx_t_3, __pyx_n_s_middle_poisson, __pyx_t_2) < 0) __PYX_ERR(0, 712, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "Fortuna.pyx":702
+  /* "Fortuna.pyx":717
  *         )
  * 
  *     def back_poisson(self, *args, **kwargs):             # <<<<<<<<<<<<<<
  *         return flatten(
  *             self.data[_back_poisson(self.size)], *args, flat=self.flat, **kwargs
  */
-  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_7Fortuna_12QuantumMonty_31back_poisson, 0, __pyx_n_s_QuantumMonty_back_poisson, NULL, __pyx_n_s_Fortuna, __pyx_d, ((PyObject *)__pyx_codeobj__108)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 702, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_4);
-  if (__Pyx_SetNameInClass(__pyx_t_3, __pyx_n_s_back_poisson, __pyx_t_4) < 0) __PYX_ERR(0, 702, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_7Fortuna_12QuantumMonty_31back_poisson, 0, __pyx_n_s_QuantumMonty_back_poisson, NULL, __pyx_n_s_Fortuna, __pyx_d, ((PyObject *)__pyx_codeobj__111)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 717, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  if (__Pyx_SetNameInClass(__pyx_t_3, __pyx_n_s_back_poisson, __pyx_t_2) < 0) __PYX_ERR(0, 717, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "Fortuna.pyx":707
+  /* "Fortuna.pyx":722
  *         )
  * 
  *     def quantum_poisson(self, *args, **kwargs):             # <<<<<<<<<<<<<<
  *         return flatten(
  *             self.data[_quantum_poisson(self.size)], *args, flat=self.flat, **kwargs
  */
-  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_7Fortuna_12QuantumMonty_33quantum_poisson, 0, __pyx_n_s_QuantumMonty_quantum_poisson, NULL, __pyx_n_s_Fortuna, __pyx_d, ((PyObject *)__pyx_codeobj__109)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 707, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_4);
-  if (__Pyx_SetNameInClass(__pyx_t_3, __pyx_n_s_quantum_poisson, __pyx_t_4) < 0) __PYX_ERR(0, 707, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_7Fortuna_12QuantumMonty_33quantum_poisson, 0, __pyx_n_s_QuantumMonty_quantum_poisson, NULL, __pyx_n_s_Fortuna, __pyx_d, ((PyObject *)__pyx_codeobj__112)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 722, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  if (__Pyx_SetNameInClass(__pyx_t_3, __pyx_n_s_quantum_poisson, __pyx_t_2) < 0) __PYX_ERR(0, 722, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "Fortuna.pyx":712
+  /* "Fortuna.pyx":727
  *         )
  * 
  *     def quantum_monty(self, *args, **kwargs):             # <<<<<<<<<<<<<<
  *         return flatten(
  *             self.data[_quantum_monty(self.size)], *args, flat=self.flat, **kwargs
  */
-  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_7Fortuna_12QuantumMonty_35quantum_monty, 0, __pyx_n_s_QuantumMonty_quantum_monty, NULL, __pyx_n_s_Fortuna, __pyx_d, ((PyObject *)__pyx_codeobj__110)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 712, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_4);
-  if (__Pyx_SetNameInClass(__pyx_t_3, __pyx_n_s_quantum_monty, __pyx_t_4) < 0) __PYX_ERR(0, 712, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_7Fortuna_12QuantumMonty_35quantum_monty, 0, __pyx_n_s_QuantumMonty_quantum_monty, NULL, __pyx_n_s_Fortuna, __pyx_d, ((PyObject *)__pyx_codeobj__113)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 727, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  if (__Pyx_SetNameInClass(__pyx_t_3, __pyx_n_s_quantum_monty, __pyx_t_2) < 0) __PYX_ERR(0, 727, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "Fortuna.pyx":595
+  /* "Fortuna.pyx":610
  * 
  * 
  * class QuantumMonty:             # <<<<<<<<<<<<<<
  *     """ Quantum Monty
  *     @param collection : Collection of Values.
  */
-  __pyx_t_4 = __Pyx_Py3ClassCreate(((PyObject*)&PyType_Type), __pyx_n_s_QuantumMonty, __pyx_empty_tuple, __pyx_t_3, NULL, 0, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 595, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_4);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_QuantumMonty, __pyx_t_4) < 0) __PYX_ERR(0, 595, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  __pyx_t_2 = __Pyx_Py3ClassCreate(((PyObject*)&PyType_Type), __pyx_n_s_QuantumMonty, __pyx_empty_tuple, __pyx_t_3, NULL, 0, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 610, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_QuantumMonty, __pyx_t_2) < 0) __PYX_ERR(0, 610, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "Fortuna.pyx":718
+  /* "Fortuna.pyx":733
  * 
  * 
  * class FlexCat:             # <<<<<<<<<<<<<<
  *     """ Flex Cat
  *     FlexCat is a lot like a multidimensional QuantumMonty.
  */
-  __pyx_t_3 = __Pyx_Py3MetaclassPrepare((PyObject *) NULL, __pyx_empty_tuple, __pyx_n_s_FlexCat, __pyx_n_s_FlexCat, (PyObject *) NULL, __pyx_n_s_Fortuna, __pyx_kp_s_Flex_Cat_FlexCat_is_a_lot_like); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 718, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_Py3MetaclassPrepare((PyObject *) NULL, __pyx_empty_tuple, __pyx_n_s_FlexCat, __pyx_n_s_FlexCat, (PyObject *) NULL, __pyx_n_s_Fortuna, __pyx_kp_s_Flex_Cat_FlexCat_is_a_lot_like); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 733, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
 
-  /* "Fortuna.pyx":738
+  /* "Fortuna.pyx":753
  *     Please refer to https://pypi.org/project/Fortuna/ for full documentation.
  *     """
  *     __slots__ = ("random_cat", "random_selection", "cat_keys", "matrix_data",             # <<<<<<<<<<<<<<
  *                  "double_cycle", "cycle")
  * 
  */
-  if (__Pyx_SetNameInClass(__pyx_t_3, __pyx_n_s_slots, __pyx_tuple__111) < 0) __PYX_ERR(0, 738, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_3, __pyx_n_s_slots, __pyx_tuple__114) < 0) __PYX_ERR(0, 753, __pyx_L1_error)
 
-  /* "Fortuna.pyx":741
+  /* "Fortuna.pyx":756
  *                  "double_cycle", "cycle")
  * 
  *     def __init__(self,             # <<<<<<<<<<<<<<
  *                  matrix_data: Dict,
  *                  key_bias: str = "front_linear",
  */
-  __pyx_t_4 = __Pyx_PyDict_NewPresized(4); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 741, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_4);
-  if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_matrix_data, __pyx_n_s_Dict) < 0) __PYX_ERR(0, 741, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_key_bias, __pyx_n_s_str) < 0) __PYX_ERR(0, 741, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_val_bias, __pyx_n_s_str) < 0) __PYX_ERR(0, 741, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_flat, __pyx_n_s_bool) < 0) __PYX_ERR(0, 741, __pyx_L1_error)
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_7Fortuna_7FlexCat_1__init__, 0, __pyx_n_s_FlexCat___init, NULL, __pyx_n_s_Fortuna, __pyx_d, ((PyObject *)__pyx_codeobj__113)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 741, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyDict_NewPresized(4); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 756, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_2, __pyx_tuple__114);
-  __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_2, __pyx_t_4);
-  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (__Pyx_SetNameInClass(__pyx_t_3, __pyx_n_s_init, __pyx_t_2) < 0) __PYX_ERR(0, 741, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_matrix_data, __pyx_n_s_Dict) < 0) __PYX_ERR(0, 756, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_key_bias, __pyx_n_s_str) < 0) __PYX_ERR(0, 756, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_val_bias, __pyx_n_s_str) < 0) __PYX_ERR(0, 756, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_flat, __pyx_n_s_bool) < 0) __PYX_ERR(0, 756, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_7Fortuna_7FlexCat_1__init__, 0, __pyx_n_s_FlexCat___init, NULL, __pyx_n_s_Fortuna, __pyx_d, ((PyObject *)__pyx_codeobj__116)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 756, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_4, __pyx_tuple__117);
+  __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_4, __pyx_t_2);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  if (__Pyx_SetNameInClass(__pyx_t_3, __pyx_n_s_init, __pyx_t_4) < 0) __PYX_ERR(0, 756, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "Fortuna.pyx":775
+  /* "Fortuna.pyx":790
  *         self.cycle = cycle(cycle_source)
  * 
  *     def __call__(self, cat_key=None, *args, **kwargs):             # <<<<<<<<<<<<<<
  *         """
  *         @param cat_key : Optional String. Default is None.
  */
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_7Fortuna_7FlexCat_3__call__, 0, __pyx_n_s_FlexCat___call, NULL, __pyx_n_s_Fortuna, __pyx_d, ((PyObject *)__pyx_codeobj__116)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 775, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_2, __pyx_tuple__117);
-  if (__Pyx_SetNameInClass(__pyx_t_3, __pyx_n_s_call, __pyx_t_2) < 0) __PYX_ERR(0, 775, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_7Fortuna_7FlexCat_3__call__, 0, __pyx_n_s_FlexCat___call, NULL, __pyx_n_s_Fortuna, __pyx_d, ((PyObject *)__pyx_codeobj__119)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 790, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_4, __pyx_tuple__120);
+  if (__Pyx_SetNameInClass(__pyx_t_3, __pyx_n_s_call, __pyx_t_4) < 0) __PYX_ERR(0, 790, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "Fortuna.pyx":718
+  /* "Fortuna.pyx":733
  * 
  * 
  * class FlexCat:             # <<<<<<<<<<<<<<
  *     """ Flex Cat
  *     FlexCat is a lot like a multidimensional QuantumMonty.
  */
-  __pyx_t_2 = __Pyx_Py3ClassCreate(((PyObject*)&PyType_Type), __pyx_n_s_FlexCat, __pyx_empty_tuple, __pyx_t_3, NULL, 0, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 718, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_FlexCat, __pyx_t_2) < 0) __PYX_ERR(0, 718, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __pyx_t_4 = __Pyx_Py3ClassCreate(((PyObject*)&PyType_Type), __pyx_n_s_FlexCat, __pyx_empty_tuple, __pyx_t_3, NULL, 0, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 733, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_FlexCat, __pyx_t_4) < 0) __PYX_ERR(0, 733, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "Fortuna.pyx":791
+  /* "Fortuna.pyx":806
  * 
  * 
  * class WeightedChoice:             # <<<<<<<<<<<<<<
  *     """ Weighted Choice
  *     Base Class, internal only.
  */
-  __pyx_t_3 = __Pyx_Py3MetaclassPrepare((PyObject *) NULL, __pyx_empty_tuple, __pyx_n_s_WeightedChoice, __pyx_n_s_WeightedChoice, (PyObject *) NULL, __pyx_n_s_Fortuna, __pyx_kp_s_Weighted_Choice_Base_Class_inte); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 791, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_Py3MetaclassPrepare((PyObject *) NULL, __pyx_empty_tuple, __pyx_n_s_WeightedChoice, __pyx_n_s_WeightedChoice, (PyObject *) NULL, __pyx_n_s_Fortuna, __pyx_kp_s_Weighted_Choice_Base_Class_inte); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 806, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
 
-  /* "Fortuna.pyx":807
+  /* "Fortuna.pyx":822
  *     Please refer to https://pypi.org/project/Fortuna/ for full documentation.
  *     """
  *     __slots__ = ("flat", "max_weight", "data")             # <<<<<<<<<<<<<<
  * 
  *     def __call__(self, *args, **kwargs):
  */
-  if (__Pyx_SetNameInClass(__pyx_t_3, __pyx_n_s_slots, __pyx_tuple__118) < 0) __PYX_ERR(0, 807, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_3, __pyx_n_s_slots, __pyx_tuple__121) < 0) __PYX_ERR(0, 822, __pyx_L1_error)
 
-  /* "Fortuna.pyx":809
+  /* "Fortuna.pyx":824
  *     __slots__ = ("flat", "max_weight", "data")
  * 
  *     def __call__(self, *args, **kwargs):             # <<<<<<<<<<<<<<
  *         """
  *         @param *args, **kwargs : Optional arguments
  */
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_7Fortuna_14WeightedChoice_1__call__, 0, __pyx_n_s_WeightedChoice___call, NULL, __pyx_n_s_Fortuna, __pyx_d, ((PyObject *)__pyx_codeobj__120)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 809, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  if (__Pyx_SetNameInClass(__pyx_t_3, __pyx_n_s_call, __pyx_t_2) < 0) __PYX_ERR(0, 809, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_7Fortuna_14WeightedChoice_1__call__, 0, __pyx_n_s_WeightedChoice___call, NULL, __pyx_n_s_Fortuna, __pyx_d, ((PyObject *)__pyx_codeobj__123)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 824, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  if (__Pyx_SetNameInClass(__pyx_t_3, __pyx_n_s_call, __pyx_t_4) < 0) __PYX_ERR(0, 824, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "Fortuna.pyx":791
+  /* "Fortuna.pyx":806
  * 
  * 
  * class WeightedChoice:             # <<<<<<<<<<<<<<
  *     """ Weighted Choice
  *     Base Class, internal only.
  */
-  __pyx_t_2 = __Pyx_Py3ClassCreate(((PyObject*)&PyType_Type), __pyx_n_s_WeightedChoice, __pyx_empty_tuple, __pyx_t_3, NULL, 0, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 791, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_WeightedChoice, __pyx_t_2) < 0) __PYX_ERR(0, 791, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __pyx_t_4 = __Pyx_Py3ClassCreate(((PyObject*)&PyType_Type), __pyx_n_s_WeightedChoice, __pyx_empty_tuple, __pyx_t_3, NULL, 0, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 806, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_WeightedChoice, __pyx_t_4) < 0) __PYX_ERR(0, 806, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "Fortuna.pyx":822
+  /* "Fortuna.pyx":837
  * 
  * 
  * class RelativeWeightedChoice(WeightedChoice):             # <<<<<<<<<<<<<<
  *     """ Relative Weighted Choice """
  *     __slots__ = ("flat", "max_weight", "data")
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_WeightedChoice); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 822, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_WeightedChoice); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 837, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_2 = PyTuple_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 822, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
+  __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 837, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
   __Pyx_GIVEREF(__pyx_t_3);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_t_3)) __PYX_ERR(0, 822, __pyx_L1_error);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_3)) __PYX_ERR(0, 837, __pyx_L1_error);
   __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_PEP560_update_bases(__pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 822, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PEP560_update_bases(__pyx_t_4); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 837, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = __Pyx_CalculateMetaclass(NULL, __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 822, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_5 = __Pyx_Py3MetaclassPrepare(__pyx_t_4, __pyx_t_3, __pyx_n_s_RelativeWeightedChoice, __pyx_n_s_RelativeWeightedChoice, (PyObject *) NULL, __pyx_n_s_Fortuna, __pyx_kp_s_Relative_Weighted_Choice); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 822, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CalculateMetaclass(NULL, __pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 837, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __pyx_t_5 = __Pyx_Py3MetaclassPrepare(__pyx_t_2, __pyx_t_3, __pyx_n_s_RelativeWeightedChoice, __pyx_n_s_RelativeWeightedChoice, (PyObject *) NULL, __pyx_n_s_Fortuna, __pyx_kp_s_Relative_Weighted_Choice); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 837, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  if (__pyx_t_3 != __pyx_t_2) {
-    if (unlikely((PyDict_SetItemString(__pyx_t_5, "__orig_bases__", __pyx_t_2) < 0))) __PYX_ERR(0, 822, __pyx_L1_error)
+  if (__pyx_t_3 != __pyx_t_4) {
+    if (unlikely((PyDict_SetItemString(__pyx_t_5, "__orig_bases__", __pyx_t_4) < 0))) __PYX_ERR(0, 837, __pyx_L1_error)
   }
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "Fortuna.pyx":824
+  /* "Fortuna.pyx":839
  * class RelativeWeightedChoice(WeightedChoice):
  *     """ Relative Weighted Choice """
  *     __slots__ = ("flat", "max_weight", "data")             # <<<<<<<<<<<<<<
  * 
  *     def __init__(self,
  */
-  if (__Pyx_SetNameInClass(__pyx_t_5, __pyx_n_s_slots, __pyx_tuple__118) < 0) __PYX_ERR(0, 824, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_5, __pyx_n_s_slots, __pyx_tuple__121) < 0) __PYX_ERR(0, 839, __pyx_L1_error)
 
-  /* "Fortuna.pyx":826
+  /* "Fortuna.pyx":841
  *     __slots__ = ("flat", "max_weight", "data")
  * 
  *     def __init__(self,             # <<<<<<<<<<<<<<
  *                  weighted_table: Iterable,
  *                  flat: bool = True):
  */
-  __pyx_t_2 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 826, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_weighted_table, __pyx_n_s_Iterable) < 0) __PYX_ERR(0, 826, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_flat, __pyx_n_s_bool) < 0) __PYX_ERR(0, 826, __pyx_L1_error)
-  __pyx_t_6 = __Pyx_CyFunction_New(&__pyx_mdef_7Fortuna_22RelativeWeightedChoice_1__init__, 0, __pyx_n_s_RelativeWeightedChoice___init_3, NULL, __pyx_n_s_Fortuna, __pyx_d, ((PyObject *)__pyx_codeobj__122)); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 826, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 841, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_weighted_table, __pyx_n_s_Iterable) < 0) __PYX_ERR(0, 841, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_flat, __pyx_n_s_bool) < 0) __PYX_ERR(0, 841, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_CyFunction_New(&__pyx_mdef_7Fortuna_22RelativeWeightedChoice_1__init__, 0, __pyx_n_s_RelativeWeightedChoice___init_3, NULL, __pyx_n_s_Fortuna, __pyx_d, ((PyObject *)__pyx_codeobj__125)); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 841, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_6, __pyx_tuple__88);
-  __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_6, __pyx_t_2);
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (__Pyx_SetNameInClass(__pyx_t_5, __pyx_n_s_init, __pyx_t_6) < 0) __PYX_ERR(0, 826, __pyx_L1_error)
+  __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_6, __pyx_t_4);
+  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  if (__Pyx_SetNameInClass(__pyx_t_5, __pyx_n_s_init, __pyx_t_6) < 0) __PYX_ERR(0, 841, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
 
-  /* "Fortuna.pyx":822
+  /* "Fortuna.pyx":837
  * 
  * 
  * class RelativeWeightedChoice(WeightedChoice):             # <<<<<<<<<<<<<<
  *     """ Relative Weighted Choice """
  *     __slots__ = ("flat", "max_weight", "data")
  */
-  __pyx_t_6 = __Pyx_Py3ClassCreate(__pyx_t_4, __pyx_n_s_RelativeWeightedChoice, __pyx_t_3, __pyx_t_5, NULL, 0, 0); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 822, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_Py3ClassCreate(__pyx_t_2, __pyx_n_s_RelativeWeightedChoice, __pyx_t_3, __pyx_t_5, NULL, 0, 0); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 837, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_RelativeWeightedChoice, __pyx_t_6) < 0) __PYX_ERR(0, 822, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_RelativeWeightedChoice, __pyx_t_6) < 0) __PYX_ERR(0, 837, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "Fortuna.pyx":848
+  /* "Fortuna.pyx":863
  * 
  * 
  * class CumulativeWeightedChoice(WeightedChoice):             # <<<<<<<<<<<<<<
  *     """ Cumulative Weighted Choice """
  *     __slots__ = ("flat", "max_weight", "data")
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_WeightedChoice); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 848, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_WeightedChoice); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 863, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 848, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_4);
+  __pyx_t_2 = PyTuple_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 863, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
   __Pyx_GIVEREF(__pyx_t_3);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_3)) __PYX_ERR(0, 848, __pyx_L1_error);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_t_3)) __PYX_ERR(0, 863, __pyx_L1_error);
   __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_PEP560_update_bases(__pyx_t_4); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 848, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PEP560_update_bases(__pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 863, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_5 = __Pyx_CalculateMetaclass(NULL, __pyx_t_3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 848, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_CalculateMetaclass(NULL, __pyx_t_3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 863, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_6 = __Pyx_Py3MetaclassPrepare(__pyx_t_5, __pyx_t_3, __pyx_n_s_CumulativeWeightedChoice, __pyx_n_s_CumulativeWeightedChoice, (PyObject *) NULL, __pyx_n_s_Fortuna, __pyx_kp_s_Cumulative_Weighted_Choice); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 848, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_Py3MetaclassPrepare(__pyx_t_5, __pyx_t_3, __pyx_n_s_CumulativeWeightedChoice, __pyx_n_s_CumulativeWeightedChoice, (PyObject *) NULL, __pyx_n_s_Fortuna, __pyx_kp_s_Cumulative_Weighted_Choice); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 863, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
-  if (__pyx_t_3 != __pyx_t_4) {
-    if (unlikely((PyDict_SetItemString(__pyx_t_6, "__orig_bases__", __pyx_t_4) < 0))) __PYX_ERR(0, 848, __pyx_L1_error)
+  if (__pyx_t_3 != __pyx_t_2) {
+    if (unlikely((PyDict_SetItemString(__pyx_t_6, "__orig_bases__", __pyx_t_2) < 0))) __PYX_ERR(0, 863, __pyx_L1_error)
   }
-  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "Fortuna.pyx":850
+  /* "Fortuna.pyx":865
  * class CumulativeWeightedChoice(WeightedChoice):
  *     """ Cumulative Weighted Choice """
  *     __slots__ = ("flat", "max_weight", "data")             # <<<<<<<<<<<<<<
  * 
  *     def __init__(self,
  */
-  if (__Pyx_SetNameInClass(__pyx_t_6, __pyx_n_s_slots, __pyx_tuple__118) < 0) __PYX_ERR(0, 850, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_6, __pyx_n_s_slots, __pyx_tuple__121) < 0) __PYX_ERR(0, 865, __pyx_L1_error)
 
-  /* "Fortuna.pyx":852
+  /* "Fortuna.pyx":867
  *     __slots__ = ("flat", "max_weight", "data")
  * 
  *     def __init__(self,             # <<<<<<<<<<<<<<
  *                  weighted_table: Iterable,
  *                  flat: bool = True):
  */
-  __pyx_t_4 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 852, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_4);
-  if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_weighted_table, __pyx_n_s_Iterable) < 0) __PYX_ERR(0, 852, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_flat, __pyx_n_s_bool) < 0) __PYX_ERR(0, 852, __pyx_L1_error)
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_7Fortuna_24CumulativeWeightedChoice_1__init__, 0, __pyx_n_s_CumulativeWeightedChoice___init_3, NULL, __pyx_n_s_Fortuna, __pyx_d, ((PyObject *)__pyx_codeobj__124)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 852, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 867, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_2, __pyx_tuple__88);
-  __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_2, __pyx_t_4);
-  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (__Pyx_SetNameInClass(__pyx_t_6, __pyx_n_s_init, __pyx_t_2) < 0) __PYX_ERR(0, 852, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_weighted_table, __pyx_n_s_Iterable) < 0) __PYX_ERR(0, 867, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_flat, __pyx_n_s_bool) < 0) __PYX_ERR(0, 867, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_7Fortuna_24CumulativeWeightedChoice_1__init__, 0, __pyx_n_s_CumulativeWeightedChoice___init_3, NULL, __pyx_n_s_Fortuna, __pyx_d, ((PyObject *)__pyx_codeobj__127)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 867, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_4, __pyx_tuple__88);
+  __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_4, __pyx_t_2);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  if (__Pyx_SetNameInClass(__pyx_t_6, __pyx_n_s_init, __pyx_t_4) < 0) __PYX_ERR(0, 867, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "Fortuna.pyx":848
+  /* "Fortuna.pyx":863
  * 
  * 
  * class CumulativeWeightedChoice(WeightedChoice):             # <<<<<<<<<<<<<<
  *     """ Cumulative Weighted Choice """
  *     __slots__ = ("flat", "max_weight", "data")
  */
-  __pyx_t_2 = __Pyx_Py3ClassCreate(__pyx_t_5, __pyx_n_s_CumulativeWeightedChoice, __pyx_t_3, __pyx_t_6, NULL, 0, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 848, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_CumulativeWeightedChoice, __pyx_t_2) < 0) __PYX_ERR(0, 848, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __pyx_t_4 = __Pyx_Py3ClassCreate(__pyx_t_5, __pyx_n_s_CumulativeWeightedChoice, __pyx_t_3, __pyx_t_6, NULL, 0, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 863, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_CumulativeWeightedChoice, __pyx_t_4) < 0) __PYX_ERR(0, 863, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "Fortuna.pyx":877
+  /* "Fortuna.pyx":892
  * 
  * 
  * class MultiChoice:             # <<<<<<<<<<<<<<
  *     """ Multiple Choice
  *     MultiChoice: generates multiple choice style questions on the terminal. """
  */
-  __pyx_t_3 = __Pyx_Py3MetaclassPrepare((PyObject *) NULL, __pyx_empty_tuple, __pyx_n_s_MultiChoice, __pyx_n_s_MultiChoice, (PyObject *) NULL, __pyx_n_s_Fortuna, __pyx_kp_s_Multiple_Choice_MultiChoice_gen); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 877, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_Py3MetaclassPrepare((PyObject *) NULL, __pyx_empty_tuple, __pyx_n_s_MultiChoice, __pyx_n_s_MultiChoice, (PyObject *) NULL, __pyx_n_s_Fortuna, __pyx_kp_s_Multiple_Choice_MultiChoice_gen); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 892, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
 
-  /* "Fortuna.pyx":881
+  /* "Fortuna.pyx":896
  *     MultiChoice: generates multiple choice style questions on the terminal. """
  * 
  *     def __init__(self,             # <<<<<<<<<<<<<<
  *                  query: str,
  *                  *,
  */
-  __pyx_t_5 = __Pyx_PyDict_NewPresized(4); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 881, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyDict_NewPresized(4); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 896, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_options, ((PyObject*)__pyx_empty_tuple)) < 0) __PYX_ERR(0, 881, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_default, ((PyObject*)__pyx_kp_u__2)) < 0) __PYX_ERR(0, 881, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_strict, ((PyObject *)Py_False)) < 0) __PYX_ERR(0, 881, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_cursor, ((PyObject*)__pyx_kp_u__3)) < 0) __PYX_ERR(0, 881, __pyx_L1_error)
-  __pyx_t_6 = __Pyx_PyDict_NewPresized(5); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 881, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_options, ((PyObject*)__pyx_empty_tuple)) < 0) __PYX_ERR(0, 896, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_default, ((PyObject*)__pyx_kp_u__2)) < 0) __PYX_ERR(0, 896, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_strict, ((PyObject *)Py_False)) < 0) __PYX_ERR(0, 896, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_cursor, ((PyObject*)__pyx_kp_u__3)) < 0) __PYX_ERR(0, 896, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyDict_NewPresized(5); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 896, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
-  if (PyDict_SetItem(__pyx_t_6, __pyx_n_s_query, __pyx_n_s_str) < 0) __PYX_ERR(0, 881, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_6, __pyx_n_s_options, __pyx_kp_s_Iterable_str) < 0) __PYX_ERR(0, 881, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_6, __pyx_n_s_default, __pyx_n_s_str) < 0) __PYX_ERR(0, 881, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_6, __pyx_n_s_strict, __pyx_n_s_bool) < 0) __PYX_ERR(0, 881, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_6, __pyx_n_s_cursor, __pyx_n_s_str) < 0) __PYX_ERR(0, 881, __pyx_L1_error)
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_7Fortuna_11MultiChoice_1__init__, 0, __pyx_n_s_MultiChoice___init, NULL, __pyx_n_s_Fortuna, __pyx_d, ((PyObject *)__pyx_codeobj__126)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 881, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __Pyx_CyFunction_SetDefaultsKwDict(__pyx_t_2, __pyx_t_5);
-  __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_2, __pyx_t_6);
+  if (PyDict_SetItem(__pyx_t_6, __pyx_n_s_query, __pyx_n_s_str) < 0) __PYX_ERR(0, 896, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_6, __pyx_n_s_options, __pyx_kp_s_Iterable_str) < 0) __PYX_ERR(0, 896, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_6, __pyx_n_s_default, __pyx_n_s_str) < 0) __PYX_ERR(0, 896, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_6, __pyx_n_s_strict, __pyx_n_s_bool) < 0) __PYX_ERR(0, 896, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_6, __pyx_n_s_cursor, __pyx_n_s_str) < 0) __PYX_ERR(0, 896, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_7Fortuna_11MultiChoice_1__init__, 0, __pyx_n_s_MultiChoice___init, NULL, __pyx_n_s_Fortuna, __pyx_d, ((PyObject *)__pyx_codeobj__129)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 896, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __Pyx_CyFunction_SetDefaultsKwDict(__pyx_t_4, __pyx_t_5);
+  __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_4, __pyx_t_6);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  if (__Pyx_SetNameInClass(__pyx_t_3, __pyx_n_s_init, __pyx_t_2) < 0) __PYX_ERR(0, 881, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  if (__Pyx_SetNameInClass(__pyx_t_3, __pyx_n_s_init, __pyx_t_4) < 0) __PYX_ERR(0, 896, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "Fortuna.pyx":916
+  /* "Fortuna.pyx":931
  *         )
  * 
  *     def _get_answer(self) -> str:             # <<<<<<<<<<<<<<
  *         return input('\n'.join(self.choice_pack)).lower() or self.default
  * 
  */
-  __pyx_t_2 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 916, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_return, __pyx_n_s_str) < 0) __PYX_ERR(0, 916, __pyx_L1_error)
-  __pyx_t_6 = __Pyx_CyFunction_New(&__pyx_mdef_7Fortuna_11MultiChoice_3_get_answer, 0, __pyx_n_s_MultiChoice__get_answer, NULL, __pyx_n_s_Fortuna, __pyx_d, ((PyObject *)__pyx_codeobj__127)); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 916, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 931, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_return, __pyx_n_s_str) < 0) __PYX_ERR(0, 931, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_CyFunction_New(&__pyx_mdef_7Fortuna_11MultiChoice_3_get_answer, 0, __pyx_n_s_MultiChoice__get_answer, NULL, __pyx_n_s_Fortuna, __pyx_d, ((PyObject *)__pyx_codeobj__130)); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 931, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
-  __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_6, __pyx_t_2);
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (__Pyx_SetNameInClass(__pyx_t_3, __pyx_n_s_get_answer, __pyx_t_6) < 0) __PYX_ERR(0, 916, __pyx_L1_error)
+  __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_6, __pyx_t_4);
+  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  if (__Pyx_SetNameInClass(__pyx_t_3, __pyx_n_s_get_answer, __pyx_t_6) < 0) __PYX_ERR(0, 931, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
 
-  /* "Fortuna.pyx":919
+  /* "Fortuna.pyx":934
  *         return input('\n'.join(self.choice_pack)).lower() or self.default
  * 
  *     def __call__(self) -> str:             # <<<<<<<<<<<<<<
  *         """ @return: String. Returns the user's selection. """
  *         selection = self._get_answer()
  */
-  __pyx_t_6 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 919, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 934, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
-  if (PyDict_SetItem(__pyx_t_6, __pyx_n_s_return, __pyx_n_s_str) < 0) __PYX_ERR(0, 919, __pyx_L1_error)
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_7Fortuna_11MultiChoice_5__call__, 0, __pyx_n_s_MultiChoice___call, NULL, __pyx_n_s_Fortuna, __pyx_d, ((PyObject *)__pyx_codeobj__129)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 919, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_2, __pyx_t_6);
+  if (PyDict_SetItem(__pyx_t_6, __pyx_n_s_return, __pyx_n_s_str) < 0) __PYX_ERR(0, 934, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_7Fortuna_11MultiChoice_5__call__, 0, __pyx_n_s_MultiChoice___call, NULL, __pyx_n_s_Fortuna, __pyx_d, ((PyObject *)__pyx_codeobj__132)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 934, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_4, __pyx_t_6);
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  if (__Pyx_SetNameInClass(__pyx_t_3, __pyx_n_s_call, __pyx_t_2) < 0) __PYX_ERR(0, 919, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  if (__Pyx_SetNameInClass(__pyx_t_3, __pyx_n_s_call, __pyx_t_4) < 0) __PYX_ERR(0, 934, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "Fortuna.pyx":877
+  /* "Fortuna.pyx":892
  * 
  * 
  * class MultiChoice:             # <<<<<<<<<<<<<<
  *     """ Multiple Choice
  *     MultiChoice: generates multiple choice style questions on the terminal. """
  */
-  __pyx_t_2 = __Pyx_Py3ClassCreate(((PyObject*)&PyType_Type), __pyx_n_s_MultiChoice, __pyx_empty_tuple, __pyx_t_3, NULL, 0, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 877, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_MultiChoice, __pyx_t_2) < 0) __PYX_ERR(0, 877, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __pyx_t_4 = __Pyx_Py3ClassCreate(((PyObject*)&PyType_Type), __pyx_n_s_MultiChoice, __pyx_empty_tuple, __pyx_t_3, NULL, 0, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 892, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_MultiChoice, __pyx_t_4) < 0) __PYX_ERR(0, 892, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "Fortuna.pyx":934
+  /* "Fortuna.pyx":949
  * 
  * 
  * def beta_variate(alpha: float, beta: float) -> float:             # <<<<<<<<<<<<<<
  *     return _beta(alpha, beta)
  * 
  */
-  __pyx_t_3 = __Pyx_PyDict_NewPresized(3); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 934, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyDict_NewPresized(3); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 949, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_alpha, __pyx_n_s_float) < 0) __PYX_ERR(0, 934, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_beta, __pyx_n_s_float) < 0) __PYX_ERR(0, 934, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_return, __pyx_n_s_float) < 0) __PYX_ERR(0, 934, __pyx_L1_error)
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_7Fortuna_97beta_variate, 0, __pyx_n_s_beta_variate, NULL, __pyx_n_s_Fortuna, __pyx_d, ((PyObject *)__pyx_codeobj__131)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 934, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_2, __pyx_t_3);
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_alpha, __pyx_n_s_float) < 0) __PYX_ERR(0, 949, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_beta, __pyx_n_s_float) < 0) __PYX_ERR(0, 949, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_return, __pyx_n_s_float) < 0) __PYX_ERR(0, 949, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_7Fortuna_97beta_variate, 0, __pyx_n_s_beta_variate, NULL, __pyx_n_s_Fortuna, __pyx_d, ((PyObject *)__pyx_codeobj__134)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 949, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_4, __pyx_t_3);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_beta_variate, __pyx_t_2) < 0) __PYX_ERR(0, 934, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_beta_variate, __pyx_t_4) < 0) __PYX_ERR(0, 949, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "Fortuna.pyx":938
+  /* "Fortuna.pyx":953
  * 
  * 
  * def pareto_variate(alpha: float) -> float:             # <<<<<<<<<<<<<<
  *     return _pareto(alpha)
  * 
  */
-  __pyx_t_2 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 938, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_alpha, __pyx_n_s_float) < 0) __PYX_ERR(0, 938, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_return, __pyx_n_s_float) < 0) __PYX_ERR(0, 938, __pyx_L1_error)
-  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_7Fortuna_99pareto_variate, 0, __pyx_n_s_pareto_variate, NULL, __pyx_n_s_Fortuna, __pyx_d, ((PyObject *)__pyx_codeobj__133)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 938, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 953, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_alpha, __pyx_n_s_float) < 0) __PYX_ERR(0, 953, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_return, __pyx_n_s_float) < 0) __PYX_ERR(0, 953, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_7Fortuna_99pareto_variate, 0, __pyx_n_s_pareto_variate, NULL, __pyx_n_s_Fortuna, __pyx_d, ((PyObject *)__pyx_codeobj__136)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 953, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_3, __pyx_t_2);
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_pareto_variate, __pyx_t_3) < 0) __PYX_ERR(0, 938, __pyx_L1_error)
+  __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_3, __pyx_t_4);
+  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_pareto_variate, __pyx_t_3) < 0) __PYX_ERR(0, 953, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "Fortuna.pyx":942
+  /* "Fortuna.pyx":957
  * 
  * 
  * def vonmises_variate(mu: float, kappa: float) -> float:             # <<<<<<<<<<<<<<
  *     return _vonmises(mu, kappa)
  * 
  */
-  __pyx_t_3 = __Pyx_PyDict_NewPresized(3); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 942, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyDict_NewPresized(3); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 957, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_mu, __pyx_n_s_float) < 0) __PYX_ERR(0, 942, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_kappa, __pyx_n_s_float) < 0) __PYX_ERR(0, 942, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_return, __pyx_n_s_float) < 0) __PYX_ERR(0, 942, __pyx_L1_error)
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_7Fortuna_101vonmises_variate, 0, __pyx_n_s_vonmises_variate, NULL, __pyx_n_s_Fortuna, __pyx_d, ((PyObject *)__pyx_codeobj__135)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 942, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_2, __pyx_t_3);
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_mu, __pyx_n_s_float) < 0) __PYX_ERR(0, 957, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_kappa, __pyx_n_s_float) < 0) __PYX_ERR(0, 957, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_return, __pyx_n_s_float) < 0) __PYX_ERR(0, 957, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_7Fortuna_101vonmises_variate, 0, __pyx_n_s_vonmises_variate, NULL, __pyx_n_s_Fortuna, __pyx_d, ((PyObject *)__pyx_codeobj__138)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 957, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_4, __pyx_t_3);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_vonmises_variate, __pyx_t_2) < 0) __PYX_ERR(0, 942, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_vonmises_variate, __pyx_t_4) < 0) __PYX_ERR(0, 957, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "Fortuna.pyx":946
+  /* "Fortuna.pyx":961
  * 
  * 
  * def bernoulli_variate(ratio_of_truth: float) -> bool:             # <<<<<<<<<<<<<<
  *     return _bernoulli(ratio_of_truth) == 1
  * 
  */
-  __pyx_t_2 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 946, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_ratio_of_truth, __pyx_n_s_float) < 0) __PYX_ERR(0, 946, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_return, __pyx_n_s_bool) < 0) __PYX_ERR(0, 946, __pyx_L1_error)
-  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_7Fortuna_103bernoulli_variate, 0, __pyx_n_s_bernoulli_variate, NULL, __pyx_n_s_Fortuna, __pyx_d, ((PyObject *)__pyx_codeobj__137)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 946, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 961, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_ratio_of_truth, __pyx_n_s_float) < 0) __PYX_ERR(0, 961, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_return, __pyx_n_s_bool) < 0) __PYX_ERR(0, 961, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_7Fortuna_103bernoulli_variate, 0, __pyx_n_s_bernoulli_variate, NULL, __pyx_n_s_Fortuna, __pyx_d, ((PyObject *)__pyx_codeobj__140)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 961, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_3, __pyx_t_2);
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_bernoulli_variate, __pyx_t_3) < 0) __PYX_ERR(0, 946, __pyx_L1_error)
+  __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_3, __pyx_t_4);
+  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_bernoulli_variate, __pyx_t_3) < 0) __PYX_ERR(0, 961, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "Fortuna.pyx":950
+  /* "Fortuna.pyx":965
  * 
  * 
  * def binomial_variate(number_of_trials: int, probability: float) -> int:             # <<<<<<<<<<<<<<
  *     return _binomial(number_of_trials, probability)
  * 
  */
-  __pyx_t_3 = __Pyx_PyDict_NewPresized(3); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 950, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyDict_NewPresized(3); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 965, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_number_of_trials, __pyx_n_s_int) < 0) __PYX_ERR(0, 950, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_probability, __pyx_n_s_float) < 0) __PYX_ERR(0, 950, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_return, __pyx_n_s_int) < 0) __PYX_ERR(0, 950, __pyx_L1_error)
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_7Fortuna_105binomial_variate, 0, __pyx_n_s_binomial_variate, NULL, __pyx_n_s_Fortuna, __pyx_d, ((PyObject *)__pyx_codeobj__139)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 950, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_2, __pyx_t_3);
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_number_of_trials, __pyx_n_s_int) < 0) __PYX_ERR(0, 965, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_probability, __pyx_n_s_float) < 0) __PYX_ERR(0, 965, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_return, __pyx_n_s_int) < 0) __PYX_ERR(0, 965, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_7Fortuna_105binomial_variate, 0, __pyx_n_s_binomial_variate, NULL, __pyx_n_s_Fortuna, __pyx_d, ((PyObject *)__pyx_codeobj__142)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 965, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_4, __pyx_t_3);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_binomial_variate, __pyx_t_2) < 0) __PYX_ERR(0, 950, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_binomial_variate, __pyx_t_4) < 0) __PYX_ERR(0, 965, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "Fortuna.pyx":954
+  /* "Fortuna.pyx":969
  * 
  * 
  * def negative_binomial_variate(number_of_trials: int, probability: float) -> int:             # <<<<<<<<<<<<<<
  *     return _neg_binomial(number_of_trials, probability)
  * 
  */
-  __pyx_t_2 = __Pyx_PyDict_NewPresized(3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 954, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_number_of_trials, __pyx_n_s_int) < 0) __PYX_ERR(0, 954, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_probability, __pyx_n_s_float) < 0) __PYX_ERR(0, 954, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_return, __pyx_n_s_int) < 0) __PYX_ERR(0, 954, __pyx_L1_error)
-  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_7Fortuna_107negative_binomial_variate, 0, __pyx_n_s_negative_binomial_variate, NULL, __pyx_n_s_Fortuna, __pyx_d, ((PyObject *)__pyx_codeobj__140)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 954, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyDict_NewPresized(3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 969, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_number_of_trials, __pyx_n_s_int) < 0) __PYX_ERR(0, 969, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_probability, __pyx_n_s_float) < 0) __PYX_ERR(0, 969, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_return, __pyx_n_s_int) < 0) __PYX_ERR(0, 969, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_7Fortuna_107negative_binomial_variate, 0, __pyx_n_s_negative_binomial_variate, NULL, __pyx_n_s_Fortuna, __pyx_d, ((PyObject *)__pyx_codeobj__143)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 969, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_3, __pyx_t_2);
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_negative_binomial_variate, __pyx_t_3) < 0) __PYX_ERR(0, 954, __pyx_L1_error)
+  __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_3, __pyx_t_4);
+  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_negative_binomial_variate, __pyx_t_3) < 0) __PYX_ERR(0, 969, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "Fortuna.pyx":958
+  /* "Fortuna.pyx":973
  * 
  * 
  * def geometric_variate(probability: float) -> int:             # <<<<<<<<<<<<<<
  *     return _geometric(probability)
  * 
  */
-  __pyx_t_3 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 958, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 973, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_probability, __pyx_n_s_float) < 0) __PYX_ERR(0, 958, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_return, __pyx_n_s_int) < 0) __PYX_ERR(0, 958, __pyx_L1_error)
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_7Fortuna_109geometric_variate, 0, __pyx_n_s_geometric_variate, NULL, __pyx_n_s_Fortuna, __pyx_d, ((PyObject *)__pyx_codeobj__142)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 958, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_2, __pyx_t_3);
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_probability, __pyx_n_s_float) < 0) __PYX_ERR(0, 973, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_return, __pyx_n_s_int) < 0) __PYX_ERR(0, 973, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_7Fortuna_109geometric_variate, 0, __pyx_n_s_geometric_variate, NULL, __pyx_n_s_Fortuna, __pyx_d, ((PyObject *)__pyx_codeobj__145)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 973, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_4, __pyx_t_3);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_geometric_variate, __pyx_t_2) < 0) __PYX_ERR(0, 958, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_geometric_variate, __pyx_t_4) < 0) __PYX_ERR(0, 973, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "Fortuna.pyx":962
+  /* "Fortuna.pyx":977
  * 
  * 
  * def poisson_variate(mean: float) -> int:             # <<<<<<<<<<<<<<
  *     return _poisson(mean)
  * 
  */
-  __pyx_t_2 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 962, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_mean, __pyx_n_s_float) < 0) __PYX_ERR(0, 962, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_return, __pyx_n_s_int) < 0) __PYX_ERR(0, 962, __pyx_L1_error)
-  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_7Fortuna_111poisson_variate, 0, __pyx_n_s_poisson_variate, NULL, __pyx_n_s_Fortuna, __pyx_d, ((PyObject *)__pyx_codeobj__144)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 962, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 977, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_mean, __pyx_n_s_float) < 0) __PYX_ERR(0, 977, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_return, __pyx_n_s_int) < 0) __PYX_ERR(0, 977, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_7Fortuna_111poisson_variate, 0, __pyx_n_s_poisson_variate, NULL, __pyx_n_s_Fortuna, __pyx_d, ((PyObject *)__pyx_codeobj__147)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 977, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_3, __pyx_t_2);
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_poisson_variate, __pyx_t_3) < 0) __PYX_ERR(0, 962, __pyx_L1_error)
+  __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_3, __pyx_t_4);
+  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_poisson_variate, __pyx_t_3) < 0) __PYX_ERR(0, 977, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "Fortuna.pyx":966
+  /* "Fortuna.pyx":981
  * 
  * 
  * def exponential_variate(lambda_rate: float) -> float:             # <<<<<<<<<<<<<<
  *     return _exponential(lambda_rate)
  * 
  */
-  __pyx_t_3 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 966, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 981, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_lambda_rate, __pyx_n_s_float) < 0) __PYX_ERR(0, 966, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_return, __pyx_n_s_float) < 0) __PYX_ERR(0, 966, __pyx_L1_error)
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_7Fortuna_113exponential_variate, 0, __pyx_n_s_exponential_variate, NULL, __pyx_n_s_Fortuna, __pyx_d, ((PyObject *)__pyx_codeobj__146)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 966, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_2, __pyx_t_3);
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_lambda_rate, __pyx_n_s_float) < 0) __PYX_ERR(0, 981, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_return, __pyx_n_s_float) < 0) __PYX_ERR(0, 981, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_7Fortuna_113exponential_variate, 0, __pyx_n_s_exponential_variate, NULL, __pyx_n_s_Fortuna, __pyx_d, ((PyObject *)__pyx_codeobj__149)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 981, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_4, __pyx_t_3);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_exponential_variate, __pyx_t_2) < 0) __PYX_ERR(0, 966, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_exponential_variate, __pyx_t_4) < 0) __PYX_ERR(0, 981, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "Fortuna.pyx":970
+  /* "Fortuna.pyx":985
  * 
  * 
  * def gamma_variate(shape: float, scale: float) -> float:             # <<<<<<<<<<<<<<
  *     return _gamma(shape, scale)
  * 
  */
-  __pyx_t_2 = __Pyx_PyDict_NewPresized(3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 970, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_shape, __pyx_n_s_float) < 0) __PYX_ERR(0, 970, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_scale, __pyx_n_s_float) < 0) __PYX_ERR(0, 970, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_return, __pyx_n_s_float) < 0) __PYX_ERR(0, 970, __pyx_L1_error)
-  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_7Fortuna_115gamma_variate, 0, __pyx_n_s_gamma_variate, NULL, __pyx_n_s_Fortuna, __pyx_d, ((PyObject *)__pyx_codeobj__148)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 970, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyDict_NewPresized(3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 985, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_shape, __pyx_n_s_float) < 0) __PYX_ERR(0, 985, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_scale, __pyx_n_s_float) < 0) __PYX_ERR(0, 985, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_return, __pyx_n_s_float) < 0) __PYX_ERR(0, 985, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_7Fortuna_115gamma_variate, 0, __pyx_n_s_gamma_variate, NULL, __pyx_n_s_Fortuna, __pyx_d, ((PyObject *)__pyx_codeobj__151)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 985, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_3, __pyx_t_2);
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_gamma_variate, __pyx_t_3) < 0) __PYX_ERR(0, 970, __pyx_L1_error)
+  __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_3, __pyx_t_4);
+  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_gamma_variate, __pyx_t_3) < 0) __PYX_ERR(0, 985, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "Fortuna.pyx":974
+  /* "Fortuna.pyx":989
  * 
  * 
  * def weibull_variate(shape: float, scale: float) -> float:             # <<<<<<<<<<<<<<
  *     return _weibull(shape, scale)
  * 
  */
-  __pyx_t_3 = __Pyx_PyDict_NewPresized(3); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 974, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyDict_NewPresized(3); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 989, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_shape, __pyx_n_s_float) < 0) __PYX_ERR(0, 974, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_scale, __pyx_n_s_float) < 0) __PYX_ERR(0, 974, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_return, __pyx_n_s_float) < 0) __PYX_ERR(0, 974, __pyx_L1_error)
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_7Fortuna_117weibull_variate, 0, __pyx_n_s_weibull_variate, NULL, __pyx_n_s_Fortuna, __pyx_d, ((PyObject *)__pyx_codeobj__149)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 974, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_2, __pyx_t_3);
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_shape, __pyx_n_s_float) < 0) __PYX_ERR(0, 989, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_scale, __pyx_n_s_float) < 0) __PYX_ERR(0, 989, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_return, __pyx_n_s_float) < 0) __PYX_ERR(0, 989, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_7Fortuna_117weibull_variate, 0, __pyx_n_s_weibull_variate, NULL, __pyx_n_s_Fortuna, __pyx_d, ((PyObject *)__pyx_codeobj__152)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 989, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_4, __pyx_t_3);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_weibull_variate, __pyx_t_2) < 0) __PYX_ERR(0, 974, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_weibull_variate, __pyx_t_4) < 0) __PYX_ERR(0, 989, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "Fortuna.pyx":978
+  /* "Fortuna.pyx":993
  * 
  * 
  * def normal_variate(mean: float, std_dev: float) -> float:             # <<<<<<<<<<<<<<
  *     return _normal(mean, std_dev)
  * 
  */
-  __pyx_t_2 = __Pyx_PyDict_NewPresized(3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 978, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_mean, __pyx_n_s_float) < 0) __PYX_ERR(0, 978, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_std_dev, __pyx_n_s_float) < 0) __PYX_ERR(0, 978, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_return, __pyx_n_s_float) < 0) __PYX_ERR(0, 978, __pyx_L1_error)
-  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_7Fortuna_119normal_variate, 0, __pyx_n_s_normal_variate, NULL, __pyx_n_s_Fortuna, __pyx_d, ((PyObject *)__pyx_codeobj__151)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 978, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyDict_NewPresized(3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 993, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_mean, __pyx_n_s_float) < 0) __PYX_ERR(0, 993, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_std_dev, __pyx_n_s_float) < 0) __PYX_ERR(0, 993, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_return, __pyx_n_s_float) < 0) __PYX_ERR(0, 993, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_7Fortuna_119normal_variate, 0, __pyx_n_s_normal_variate, NULL, __pyx_n_s_Fortuna, __pyx_d, ((PyObject *)__pyx_codeobj__154)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 993, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_3, __pyx_t_2);
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_normal_variate, __pyx_t_3) < 0) __PYX_ERR(0, 978, __pyx_L1_error)
+  __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_3, __pyx_t_4);
+  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_normal_variate, __pyx_t_3) < 0) __PYX_ERR(0, 993, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "Fortuna.pyx":982
+  /* "Fortuna.pyx":997
  * 
  * 
  * def log_normal_variate(log_mean: float, log_deviation: float) -> float:             # <<<<<<<<<<<<<<
  *     return _log_normal(log_mean, log_deviation)
  * 
  */
-  __pyx_t_3 = __Pyx_PyDict_NewPresized(3); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 982, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyDict_NewPresized(3); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 997, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_log_mean, __pyx_n_s_float) < 0) __PYX_ERR(0, 982, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_log_deviation, __pyx_n_s_float) < 0) __PYX_ERR(0, 982, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_return, __pyx_n_s_float) < 0) __PYX_ERR(0, 982, __pyx_L1_error)
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_7Fortuna_121log_normal_variate, 0, __pyx_n_s_log_normal_variate, NULL, __pyx_n_s_Fortuna, __pyx_d, ((PyObject *)__pyx_codeobj__153)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 982, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_2, __pyx_t_3);
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_log_mean, __pyx_n_s_float) < 0) __PYX_ERR(0, 997, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_log_deviation, __pyx_n_s_float) < 0) __PYX_ERR(0, 997, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_return, __pyx_n_s_float) < 0) __PYX_ERR(0, 997, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_7Fortuna_121log_normal_variate, 0, __pyx_n_s_log_normal_variate, NULL, __pyx_n_s_Fortuna, __pyx_d, ((PyObject *)__pyx_codeobj__156)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 997, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_4, __pyx_t_3);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_log_normal_variate, __pyx_t_2) < 0) __PYX_ERR(0, 982, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_log_normal_variate, __pyx_t_4) < 0) __PYX_ERR(0, 997, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "Fortuna.pyx":986
+  /* "Fortuna.pyx":1001
  * 
  * 
  * def extreme_value_variate(location: float, scale: float) -> float:             # <<<<<<<<<<<<<<
  *     return _extreme_value(location, scale)
  * 
  */
-  __pyx_t_2 = __Pyx_PyDict_NewPresized(3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 986, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_location, __pyx_n_s_float) < 0) __PYX_ERR(0, 986, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_scale, __pyx_n_s_float) < 0) __PYX_ERR(0, 986, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_return, __pyx_n_s_float) < 0) __PYX_ERR(0, 986, __pyx_L1_error)
-  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_7Fortuna_123extreme_value_variate, 0, __pyx_n_s_extreme_value_variate, NULL, __pyx_n_s_Fortuna, __pyx_d, ((PyObject *)__pyx_codeobj__155)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 986, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyDict_NewPresized(3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1001, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_location, __pyx_n_s_float) < 0) __PYX_ERR(0, 1001, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_scale, __pyx_n_s_float) < 0) __PYX_ERR(0, 1001, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_return, __pyx_n_s_float) < 0) __PYX_ERR(0, 1001, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_7Fortuna_123extreme_value_variate, 0, __pyx_n_s_extreme_value_variate, NULL, __pyx_n_s_Fortuna, __pyx_d, ((PyObject *)__pyx_codeobj__158)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1001, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_3, __pyx_t_2);
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_extreme_value_variate, __pyx_t_3) < 0) __PYX_ERR(0, 986, __pyx_L1_error)
+  __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_3, __pyx_t_4);
+  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_extreme_value_variate, __pyx_t_3) < 0) __PYX_ERR(0, 1001, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "Fortuna.pyx":990
+  /* "Fortuna.pyx":1005
  * 
  * 
  * def chi_squared_variate(degrees_of_freedom: float) -> float:             # <<<<<<<<<<<<<<
  *     return _chi_squared(degrees_of_freedom)
  * 
  */
-  __pyx_t_3 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 990, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1005, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_degrees_of_freedom, __pyx_n_s_float) < 0) __PYX_ERR(0, 990, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_return, __pyx_n_s_float) < 0) __PYX_ERR(0, 990, __pyx_L1_error)
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_7Fortuna_125chi_squared_variate, 0, __pyx_n_s_chi_squared_variate, NULL, __pyx_n_s_Fortuna, __pyx_d, ((PyObject *)__pyx_codeobj__157)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 990, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_2, __pyx_t_3);
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_degrees_of_freedom, __pyx_n_s_float) < 0) __PYX_ERR(0, 1005, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_return, __pyx_n_s_float) < 0) __PYX_ERR(0, 1005, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_7Fortuna_125chi_squared_variate, 0, __pyx_n_s_chi_squared_variate, NULL, __pyx_n_s_Fortuna, __pyx_d, ((PyObject *)__pyx_codeobj__160)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1005, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_4, __pyx_t_3);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_chi_squared_variate, __pyx_t_2) < 0) __PYX_ERR(0, 990, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_chi_squared_variate, __pyx_t_4) < 0) __PYX_ERR(0, 1005, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "Fortuna.pyx":994
+  /* "Fortuna.pyx":1009
  * 
  * 
  * def cauchy_variate(location: float, scale: float) -> float:             # <<<<<<<<<<<<<<
  *     return _cauchy(location, scale)
  * 
  */
-  __pyx_t_2 = __Pyx_PyDict_NewPresized(3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 994, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_location, __pyx_n_s_float) < 0) __PYX_ERR(0, 994, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_scale, __pyx_n_s_float) < 0) __PYX_ERR(0, 994, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_return, __pyx_n_s_float) < 0) __PYX_ERR(0, 994, __pyx_L1_error)
-  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_7Fortuna_127cauchy_variate, 0, __pyx_n_s_cauchy_variate, NULL, __pyx_n_s_Fortuna, __pyx_d, ((PyObject *)__pyx_codeobj__158)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 994, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyDict_NewPresized(3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1009, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_location, __pyx_n_s_float) < 0) __PYX_ERR(0, 1009, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_scale, __pyx_n_s_float) < 0) __PYX_ERR(0, 1009, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_return, __pyx_n_s_float) < 0) __PYX_ERR(0, 1009, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_7Fortuna_127cauchy_variate, 0, __pyx_n_s_cauchy_variate, NULL, __pyx_n_s_Fortuna, __pyx_d, ((PyObject *)__pyx_codeobj__161)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1009, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_3, __pyx_t_2);
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_cauchy_variate, __pyx_t_3) < 0) __PYX_ERR(0, 994, __pyx_L1_error)
+  __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_3, __pyx_t_4);
+  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_cauchy_variate, __pyx_t_3) < 0) __PYX_ERR(0, 1009, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "Fortuna.pyx":998
+  /* "Fortuna.pyx":1013
  * 
  * 
  * def fisher_f_variate(degrees_of_freedom_1: float, degrees_of_freedom_2: float) -> float:             # <<<<<<<<<<<<<<
  *     return _fisher_f(degrees_of_freedom_1, degrees_of_freedom_2)
  * 
  */
-  __pyx_t_3 = __Pyx_PyDict_NewPresized(3); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 998, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyDict_NewPresized(3); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1013, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_degrees_of_freedom_1, __pyx_n_s_float) < 0) __PYX_ERR(0, 998, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_degrees_of_freedom_2, __pyx_n_s_float) < 0) __PYX_ERR(0, 998, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_return, __pyx_n_s_float) < 0) __PYX_ERR(0, 998, __pyx_L1_error)
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_7Fortuna_129fisher_f_variate, 0, __pyx_n_s_fisher_f_variate, NULL, __pyx_n_s_Fortuna, __pyx_d, ((PyObject *)__pyx_codeobj__160)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 998, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_2, __pyx_t_3);
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_degrees_of_freedom_1, __pyx_n_s_float) < 0) __PYX_ERR(0, 1013, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_degrees_of_freedom_2, __pyx_n_s_float) < 0) __PYX_ERR(0, 1013, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_return, __pyx_n_s_float) < 0) __PYX_ERR(0, 1013, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_7Fortuna_129fisher_f_variate, 0, __pyx_n_s_fisher_f_variate, NULL, __pyx_n_s_Fortuna, __pyx_d, ((PyObject *)__pyx_codeobj__163)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1013, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_4, __pyx_t_3);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_fisher_f_variate, __pyx_t_2) < 0) __PYX_ERR(0, 998, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_fisher_f_variate, __pyx_t_4) < 0) __PYX_ERR(0, 1013, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "Fortuna.pyx":1002
+  /* "Fortuna.pyx":1017
  * 
  * 
  * def student_t_variate(degrees_of_freedom: float) -> float:             # <<<<<<<<<<<<<<
  *     return _student_t(degrees_of_freedom)
  */
-  __pyx_t_2 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1002, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_degrees_of_freedom, __pyx_n_s_float) < 0) __PYX_ERR(0, 1002, __pyx_L1_error)
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_return, __pyx_n_s_float) < 0) __PYX_ERR(0, 1002, __pyx_L1_error)
-  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_7Fortuna_131student_t_variate, 0, __pyx_n_s_student_t_variate, NULL, __pyx_n_s_Fortuna, __pyx_d, ((PyObject *)__pyx_codeobj__161)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1002, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1017, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_degrees_of_freedom, __pyx_n_s_float) < 0) __PYX_ERR(0, 1017, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_return, __pyx_n_s_float) < 0) __PYX_ERR(0, 1017, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_7Fortuna_131student_t_variate, 0, __pyx_n_s_student_t_variate, NULL, __pyx_n_s_Fortuna, __pyx_d, ((PyObject *)__pyx_codeobj__164)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1017, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_3, __pyx_t_2);
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_student_t_variate, __pyx_t_3) < 0) __PYX_ERR(0, 1002, __pyx_L1_error)
+  __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_3, __pyx_t_4);
+  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_student_t_variate, __pyx_t_3) < 0) __PYX_ERR(0, 1017, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
   /* "Fortuna.pyx":1
  * #!python3             # <<<<<<<<<<<<<<
  * #distutils: language = c++
  * from collections import deque
  */
   __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  if (PyDict_SetItem(__pyx_t_3, __pyx_kp_u_MultiChoice___init___line_881, __pyx_kp_u_Multiple_Choice_param_query_Str) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_kp_u_MultiChoice___init___line_896, __pyx_kp_u_Multiple_Choice_param_query_Str) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_test, __pyx_t_3) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
   /*--- Wrapped vars code ---*/
 
   goto __pyx_L0;
   __pyx_L1_error:;
@@ -37885,15 +38557,15 @@
 __Pyx_PyType_GetName(PyTypeObject* tp)
 {
     PyObject *name = __Pyx_PyObject_GetAttrStr((PyObject *)tp,
                                                __pyx_n_s_name);
     if (unlikely(name == NULL) || unlikely(!PyUnicode_Check(name))) {
         PyErr_Clear();
         Py_XDECREF(name);
-        name = __Pyx_NewRef(__pyx_n_s__162);
+        name = __Pyx_NewRef(__pyx_n_s__165);
     }
     return name;
 }
 #endif
 
 /* CIntFromPy */
 static CYTHON_INLINE long __Pyx_PyInt_As_long(PyObject *x) {
```

### Comparing `fortuna-5.5.1/Fortuna.pyx` & `fortuna-5.5.2/Fortuna.pyx`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!python3
 #distutils: language = c++
 from collections import deque
 from itertools import cycle
 from math import sqrt
-from typing import Callable, Iterable, Dict
+from typing import Callable, Iterable, Dict, Iterator
 
 version = "5.5.1"
 
 cdef extern from "Storm.hpp":
     const char* _storm_version "Storm::get_version"()
     void _seed "Storm::Engine::seed"(unsigned long long)
     double _float_clamp "Storm::GearBox::clamp"(double, double, double)
@@ -545,14 +545,29 @@
         self.zero_cool = zero_cool
         self.flat = flat
 
     def __call__(self, *args, **kwargs):
         return flatten(self.data[self.zero_cool(len(self.data))], *args, flat=self.flat, **kwargs)
 
 
+class TruffleShuffle2:
+    __slots__ = ("flat", "data", "size", "pivot", "index")
+
+    def __init__(self, collection: Iterable, flat: bool = True):
+        self.flat = flat
+        self.data = list(collection) if isinstance(collection, Iterator) else collection
+        self.size = len(self.data)
+        self.pivot = int(sqrt(self.size))
+        self.index = _random_index(self.size)
+
+    def __call__(self, *args, **kwargs):
+        self.index = (self.index + 1 + _front_poisson(self.pivot)) % self.size
+        return flatten(self.data[self.index], *args, flat=self.flat, **kwargs)
+
+
 class TruffleShuffle:
     """ Truffle Shuffle
     Produces random values from a collection with a Wide Uniform Distribution.
 
     @param collection : Collection of Values. Any list-like object, a Set is
         recommended but not required.
     @param flat : Bool. Default: True. Option to automatically flatten
```

### Comparing `fortuna-5.5.1/LICENSE` & `fortuna-5.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `fortuna-5.5.1/setup.py` & `fortuna-5.5.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
         compiler_directives={
             "embedsignature": True,
             "language_level": 3,
         },
     ),
     author="Robert Sharp",
     author_email="webmaster@sharpdesigndigital.com",
-    version="5.5.1",
+    version="5.5.2",
     description="High Performance Random Value Toolkit",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license="Free for non-commercial use",
     platforms=["Darwin", "Linux", "Windows"],
     extras_require={
         'scope': ['MonkeyScope>=1.5.0'],
```

