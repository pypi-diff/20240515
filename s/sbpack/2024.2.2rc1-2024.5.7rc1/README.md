# Comparing `tmp/sbpack-2024.2.2rc1-py3-none-any.whl.zip` & `tmp/sbpack-2024.5.7rc1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,26 +1,27 @@
-Zip file size: 40627 bytes, number of entries: 24
+Zip file size: 37039 bytes, number of entries: 25
 -rw-r--r--  2.0 unx        0 b- defN 23-May-09 11:19 sbpack/__init__.py
 -rw-r--r--  2.0 unx     5754 b- defN 24-Jan-30 09:16 sbpack/lib.py
 -rw-r--r--  2.0 unx    13554 b- defN 24-Feb-02 10:09 sbpack/pack.py
 -rw-r--r--  2.0 unx     7929 b- defN 23-Jun-22 11:09 sbpack/schemadef.py
 -rw-r--r--  2.0 unx     3064 b- defN 23-May-09 11:19 sbpack/unpack.py
--rw-r--r--  2.0 unx       28 b- defN 24-Feb-02 10:10 sbpack/version.py
--rw-r--r--  2.0 unx      240 b- defN 24-Jan-03 14:54 sbpack/noncwl/__init__.py
--rw-r--r--  2.0 unx     3965 b- defN 24-Jan-05 12:56 sbpack/noncwl/constants.py
+-rw-r--r--  2.0 unx       28 b- defN 24-May-07 12:13 sbpack/version.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-24 14:38 sbpack/noncwl/__init__.py
+-rw-r--r--  2.0 unx     2247 b- defN 24-May-09 08:30 sbpack/noncwl/constants.py
 -rw-r--r--  2.0 unx     1591 b- defN 23-May-09 11:19 sbpack/noncwl/copy.py
 -rw-r--r--  2.0 unx     3755 b- defN 23-Sep-27 08:59 sbpack/noncwl/copy_app.py
--rw-r--r--  2.0 unx    24043 b- defN 24-Jan-30 09:15 sbpack/noncwl/nextflow.py
--rw-r--r--  2.0 unx    13423 b- defN 24-Jan-17 13:33 sbpack/noncwl/utils.py
--rw-r--r--  2.0 unx    10243 b- defN 23-Nov-06 14:52 sbpack/noncwl/wdl.py
+-rw-r--r--  2.0 unx     9768 b- defN 24-May-14 15:50 sbpack/noncwl/manifest.py
+-rw-r--r--  2.0 unx     9540 b- defN 24-May-09 08:30 sbpack/noncwl/nextflow.py
+-rw-r--r--  2.0 unx     5456 b- defN 24-May-09 08:37 sbpack/noncwl/utils.py
+-rw-r--r--  2.0 unx    10279 b- defN 24-Apr-24 15:07 sbpack/noncwl/wdl.py
 -rw-r--r--  2.0 unx     6360 b- defN 24-Jan-05 13:12 sbpack/noncwl/wrapper.py
 -rw-r--r--  2.0 unx     3667 b- defN 24-Jan-03 12:14 sbpack/noncwl/js/sample_sheet_generator.js
 -rw-r--r--  2.0 unx      197 b- defN 24-Jan-03 12:14 sbpack/noncwl/js/sample_sheet_switch.js
--rw-r--r--  2.0 unx     3971 b- defN 24-Jan-04 15:00 sbpack/noncwl/js_templates/sample_sheet_generator.js
+-rw-r--r--  2.0 unx     3946 b- defN 24-Mar-13 14:30 sbpack/noncwl/js_templates/sample_sheet_generator.js
 -rw-r--r--  2.0 unx      192 b- defN 24-Jan-03 14:54 sbpack/noncwl/js_templates/sample_sheet_switch.js
--rw-r--r--  2.0 unx    11357 b- defN 24-Feb-02 10:34 sbpack-2024.2.2rc1.dist-info/LICENSE
--rw-r--r--  2.0 unx     7501 b- defN 24-Feb-02 10:34 sbpack-2024.2.2rc1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Feb-02 10:34 sbpack-2024.2.2rc1.dist-info/WHEEL
--rw-r--r--  2.0 unx      218 b- defN 24-Feb-02 10:34 sbpack-2024.2.2rc1.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        7 b- defN 24-Feb-02 10:34 sbpack-2024.2.2rc1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     2001 b- defN 24-Feb-02 10:34 sbpack-2024.2.2rc1.dist-info/RECORD
-24 files, 123152 bytes uncompressed, 37389 bytes compressed:  69.6%
+-rw-r--r--  2.0 unx    11357 b- defN 24-May-15 08:47 sbpack-2024.5.7rc1.dist-info/LICENSE
+-rw-r--r--  2.0 unx     7534 b- defN 24-May-15 08:47 sbpack-2024.5.7rc1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-15 08:47 sbpack-2024.5.7rc1.dist-info/WHEEL
+-rw-r--r--  2.0 unx      259 b- defN 24-May-15 08:47 sbpack-2024.5.7rc1.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        7 b- defN 24-May-15 08:47 sbpack-2024.5.7rc1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     2079 b- defN 24-May-15 08:47 sbpack-2024.5.7rc1.dist-info/RECORD
+25 files, 108655 bytes uncompressed, 33675 bytes compressed:  69.0%
```

## zipnote {}

```diff
@@ -24,14 +24,17 @@
 
 Filename: sbpack/noncwl/copy.py
 Comment: 
 
 Filename: sbpack/noncwl/copy_app.py
 Comment: 
 
+Filename: sbpack/noncwl/manifest.py
+Comment: 
+
 Filename: sbpack/noncwl/nextflow.py
 Comment: 
 
 Filename: sbpack/noncwl/utils.py
 Comment: 
 
 Filename: sbpack/noncwl/wdl.py
@@ -48,26 +51,26 @@
 
 Filename: sbpack/noncwl/js_templates/sample_sheet_generator.js
 Comment: 
 
 Filename: sbpack/noncwl/js_templates/sample_sheet_switch.js
 Comment: 
 
-Filename: sbpack-2024.2.2rc1.dist-info/LICENSE
+Filename: sbpack-2024.5.7rc1.dist-info/LICENSE
 Comment: 
 
-Filename: sbpack-2024.2.2rc1.dist-info/METADATA
+Filename: sbpack-2024.5.7rc1.dist-info/METADATA
 Comment: 
 
-Filename: sbpack-2024.2.2rc1.dist-info/WHEEL
+Filename: sbpack-2024.5.7rc1.dist-info/WHEEL
 Comment: 
 
-Filename: sbpack-2024.2.2rc1.dist-info/entry_points.txt
+Filename: sbpack-2024.5.7rc1.dist-info/entry_points.txt
 Comment: 
 
-Filename: sbpack-2024.2.2rc1.dist-info/top_level.txt
+Filename: sbpack-2024.5.7rc1.dist-info/top_level.txt
 Comment: 
 
-Filename: sbpack-2024.2.2rc1.dist-info/RECORD
+Filename: sbpack-2024.5.7rc1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## sbpack/version.py

```diff
@@ -1 +1 @@
-__version__ = "2024.2.2rc1"
+__version__ = "2024.5.7rc1"
```

## sbpack/noncwl/__init__.py

```diff
@@ -1,15 +0,0 @@
-00000000: 696d 706f 7274 206f 730a 0a50 4143 4b41  import os..PACKA
-00000010: 4745 5f50 4154 4820 3d20 6f73 2e70 6174  GE_PATH = os.pat
-00000020: 682e 6162 7370 6174 6828 6f73 2e70 6174  h.abspath(os.pat
-00000030: 682e 6469 726e 616d 6528 5f5f 6669 6c65  h.dirname(__file
-00000040: 5f5f 2929 0a4a 535f 5041 5448 203d 206f  __)).JS_PATH = o
-00000050: 732e 7061 7468 2e6a 6f69 6e28 5041 434b  s.path.join(PACK
-00000060: 4147 455f 5041 5448 2c20 276a 735f 7465  AGE_PATH, 'js_te
-00000070: 6d70 6c61 7465 7327 290a 0a0a 6465 6620  mplates')...def 
-00000080: 7265 6164 5f6a 735f 7465 6d70 6c61 7465  read_js_template
-00000090: 2866 696c 655f 6e61 6d65 293a 0a20 2020  (file_name):.   
-000000a0: 2077 6974 6820 6f70 656e 286f 732e 7061   with open(os.pa
-000000b0: 7468 2e6a 6f69 6e28 4a53 5f50 4154 482c  th.join(JS_PATH,
-000000c0: 2066 696c 655f 6e61 6d65 292c 2027 7227   file_name), 'r'
-000000d0: 2920 6173 2066 3a0a 2020 2020 2020 2020  ) as f:.        
-000000e0: 7265 7475 726e 2066 2e72 6561 6428 290a  return f.read().
```

## sbpack/noncwl/constants.py

```diff
@@ -1,11 +1,7 @@
-from enum import Enum
-from sbpack.noncwl import read_js_template
-
-
 # ############################## Generic Bits ############################### #
 PACKAGE_SIZE_LIMIT = 100 * 1024 * 1024  # 100 MB
 REMOVE_INPUT_KEY = "REMOVE_THIS_KEY"
 
 
 # keep track of what extensions are applicable for processing
 class EXTENSIONS:
@@ -18,16 +14,14 @@
     json_all = [json]
     all_ = [yaml, yml, json, cwl]
 
 
 # ############################ CWL Standard Bits ############################ #
 # A generic SB input array of files that should be available on the
 # instance but are not explicitly provided to the execution as wdl params.
-SAMPLE_SHEET_FUNCTION = read_js_template("sample_sheet_generator.js")
-SAMPLE_SHEET_SWITCH = read_js_template("sample_sheet_switch.js")
 
 GENERIC_FILE_ARRAY_INPUT = {
     "id": "auxiliary_files",
     "type": "File[]?",
     "label": "Auxiliary files",
     "doc": "List of files not added as explicit workflow inputs but "
            "required for workflow execution."
@@ -37,26 +31,14 @@
     "id": "file_input",
     "type": "File[]?",
     "label": "Input files",
     "doc": "List of files that will be used to autogenerate the sample sheet "
            "that is required for workflow execution."
 }
 
-GENERIC_NF_OUTPUT_DIRECTORY = {
-    "id": "nf_workdir",
-    "type": "Directory?",
-    "label": "Work Directory",
-    "doc": "This is a template output. "
-           "Please change glob to directories specified in "
-           "publishDir in the workflow.",
-    "outputBinding": {
-        "glob": "work"
-    }
-}
-
 GENERIC_WDL_OUTPUT_DIRECTORY = {
     "id": "output_txt",
     "doc": "This is a template output. "
            "Please modify to collect final outputs using "
            "glob inside the working directory.",
     "type": "File[]",
     "outputBinding": {
@@ -80,66 +62,31 @@
 
 # Legacy - Delete after updating wdl.py
 WRAPPER_REQUIREMENTS = [
     INLINE_JS_REQUIREMENT,
     AUX_FILES_REQUIREMENT
 ]
 
-
-def sample_sheet(
-        file_name, sample_sheet_input, format_, input_source, header, rows,
-        defaults, group_by):
-    basename = ".".join(file_name.split(".")[:-1])
-    ext = file_name.split(".")[-1]
-    new_name = f"{basename}.new.{ext}"
-
-    return {
-        "class": "InitialWorkDirRequirement",
-        "listing": [
-            {
-                "entryname": f"${{ return {sample_sheet_input} ? {sample_sheet_input}.nameroot + '.new' + {sample_sheet_input}.nameext : '{file_name}' }}",
-                "entry": SAMPLE_SHEET_FUNCTION.format_map(locals()),
-                "writable": False
-            }
-        ]
-    }
-
-
-# ############################## Nextflow Bits ############################## #
-# Keys that should be skipped when parsing nextflow tower yaml file
-
-NF_SCHEMA_DEFAULT_NAME = 'nextflow_schema.json'
-SB_SCHEMA_DEFAULT_NAME = 'sb_nextflow_schema'
-
-# Mappings of nextflow input fields to SB input fields
-#  nextflow_key: cwl_key mapping
-NF_TO_CWL_PORT_MAP = {
-    'default': 'sbg:toolDefaultValue',
-    'description': 'label',
-    'help_text': 'doc',
-    'mimetype': 'format',
-    'fa_icon': 'sbg:icon',
-    'pattern': 'sbg:pattern',
-    'hidden': 'sbg:hidden',
-}
-
-# Mappings of nextflow definition fields to SB category fields
-#  nextflow_key: cwl_key mapping
-NF_TO_CWL_CATEGORY_MAP = {
-    'title': 'sbg:title',
-    'description': 'sbg:doc',
-    'fa_icon': 'sbg:icon',
-}
-
-# What keys to skip from the tower.yml file
-SKIP_NEXTFLOW_TOWER_KEYS = [
-    'tower',
-    'mail',
+# Nextflow
+DEFAULT_EXCLUDE_PATTERNS = [
+    "*.git",
+    "*.git*",
+    ".git",
+    ".git*",
+    # ".github",
+    # ".gitignore",
+    # ".gitpod.yml",
+    "work",
+    ".nextflow.log",
+    ".DS_Store",
+    ".devcontainer",
+    ".editorconfig",
+    ".gitattributes",
+    ".nextflow",
+    # ".nf-core.yml",
+    ".pre-commit-config.yaml",
+    ".prettierignore",
+    ".prettierrc.yml",
+    ".idea",
+    ".pytest_cache",
+    "*.egg-info",
 ]
-
-
-class ExecMode(Enum):
-    single = 'single-instance'
-    multi = 'multi-instance'
-
-    def __str__(self):
-        return self.value
```

## sbpack/noncwl/nextflow.py

```diff
@@ -1,66 +1,49 @@
-import re
-import json
 import argparse
 import logging
-import os
 import yaml
+import os
 
 import sbpack.lib as lib
-from packaging import version
+
+from wrabbit.parser.nextflow import NextflowParser
 
 from nf_core.schema import PipelineSchema
 from sbpack.version import __version__
-from sbpack.pack import pack
+
+from sbpack.noncwl.constants import (
+    DEFAULT_EXCLUDE_PATTERNS,
+)
+
 from sbpack.noncwl.utils import (
-    get_dict_depth,
     zip_and_push_to_sb,
+    install_or_upgrade_app,
+)
+
+from wrabbit.parser.utils import (
     get_readme,
-    get_tower_yml,
-    get_entrypoint,
-    get_executor_version,
     get_latest_sb_schema,
     get_sample_sheet_schema,
-    get_config_files,
-    parse_config_file,
-    create_profile_enum,
-    install_or_upgrade_app,
-    nf_to_sb_input_mapper,
 )
-from sbpack.noncwl.constants import (
-    sample_sheet,
+
+from wrabbit.parser.constants import (
     ExecMode,
-    GENERIC_FILE_ARRAY_INPUT,
-    GENERIC_NF_OUTPUT_DIRECTORY,
-    INLINE_JS_REQUIREMENT,
-    LOAD_LISTING_REQUIREMENT,
-    AUX_FILES_REQUIREMENT,
-    SKIP_NEXTFLOW_TOWER_KEYS,
     EXTENSIONS,
-    NF_TO_CWL_CATEGORY_MAP,
-    SAMPLE_SHEET_FILE_ARRAY_INPUT,
-    SAMPLE_SHEET_SWITCH,
     NF_SCHEMA_DEFAULT_NAME,
     SB_SCHEMA_DEFAULT_NAME,
-    REMOVE_INPUT_KEY,
 )
-from sbpack.noncwl.wrapper import Wrapper
 
 logger = logging.getLogger(__name__)
 logger.setLevel(logging.INFO)
 
 
-class SBNextflowWrapper:
-    def __init__(self, workflow_path, sb_doc=None):
-        self.sb_wrapper = Wrapper()
+class SBNextflowWrapper(NextflowParser):
+    def __init__(self, workflow_path, *args, **kwargs):
+        super().__init__(workflow_path, *args, **kwargs)
         self.nf_ps = PipelineSchema()
-        self.workflow_path = workflow_path
-        self.nf_schema_path = None
-        self.nf_config_files = None
-        self.sb_doc = sb_doc
 
     def nf_schema_build(self):
         """
         Build nextflow schema using nf_core schema build feature and save to
         a file
         """
         nf_schema_path = os.path.join(
@@ -76,417 +59,14 @@
             pipeline_dir=self.workflow_path,
             no_prompts=True,
             web_only=False,
             url='',
         )
         self.nf_schema_path = nf_schema_path
 
-    def generate_sb_inputs(self):
-        """
-        Generate SB inputs schema
-        """
-
-        # ## Add profiles to the input ## #
-        self.nf_config_files = get_config_files(self.workflow_path)
-
-        profiles = dict()
-
-        for path in self.nf_config_files:
-            profiles.update(parse_config_file(path))
-
-        profiles_choices = sorted(list(set(profiles.keys())))
-
-        if profiles:
-            self.sb_wrapper.safe_add_input(
-                create_profile_enum(profiles_choices)
-            )
-
-        # Optional inputs due to profiles
-        # optional_inputs = []
-        # for profile_id, profile_contents in profiles.items():
-        #     for key in profile_contents.keys():
-        #         if 'params.' in key:
-        #             input_ = key.rsplit('params.', 0)
-        #             optional_inputs.extend(input_)
-        # optional_inputs = set(optional_inputs)
-
-        # ## Add inputs ## #
-        if self.nf_schema_path:
-            with open(self.nf_schema_path, 'r') as f:
-                nf_schema = yaml.safe_load(f)
-
-            for p_key, p_value in nf_schema.get('properties', {}).items():
-                self.sb_wrapper.safe_add_input(
-                    nf_to_sb_input_mapper(p_key, p_value))
-            for def_name, definition in nf_schema.get(
-                    'definitions', {}).items():
-                # Nextflow inputs schema contains multiple definitions where
-                # each definition contains multiple properties
-                category = dict()
-
-                for nf_field, sb_field in NF_TO_CWL_CATEGORY_MAP.items():
-                    if nf_field in definition:
-                        category[sb_field] = definition[nf_field]
-
-                input_category = 'Inputs'
-                if 'title' in definition:
-                    input_category = category['sbg:title']
-
-                for port_id, port_data in definition['properties'].items():
-                    req = False
-                    # if port_id in definition.get('required', []) and \
-                    #         port_id not in optional_inputs:
-                    #     req = True
-
-                    self.sb_wrapper.safe_add_input(nf_to_sb_input_mapper(
-                        port_id,
-                        port_data,
-                        category=input_category,
-                        required=req,
-                    ))
-
-        # Add the generic file array input - auxiliary files
-        self.sb_wrapper.safe_add_input(GENERIC_FILE_ARRAY_INPUT)
-        self.sb_wrapper.add_requirement(AUX_FILES_REQUIREMENT)
-        self.sb_wrapper.add_requirement(INLINE_JS_REQUIREMENT)
-
-    def generate_sb_outputs(self):
-        """
-        Generate SB output schema
-        """
-        if get_tower_yml(self.workflow_path):
-            for output in self.parse_output_yml(
-                    open(get_tower_yml(self.workflow_path))
-            ):
-                self.sb_wrapper.safe_add_output(output)
-
-        # if the only output is reports, or there are no outputs, add generic
-        if len(self.sb_wrapper.outputs) == 0 or \
-                (len(self.sb_wrapper.outputs) == 1 and
-                 self.sb_wrapper.outputs[0]['id'] == 'reports'):
-            self.sb_wrapper.safe_add_output(GENERIC_NF_OUTPUT_DIRECTORY)
-
-    def parse_sample_sheet_schema(self, path):
-        """
-        Example sample sheet:
-        sample_sheet_input: input_sample_sheet  # taken from app wrapper
-        sample_sheet_name: samplesheet.csv
-        header:
-          - SampleID
-          - Fastq1
-          - Fastq2
-        rows:
-          - sample_id
-          - path
-          - path
-        defaults:
-          - NA
-          - NA
-          - NA
-        group_by: sample_id
-        format_: csv
-
-        """
-        schema = yaml.safe_load(path)
-
-        sample_sheet_input = schema.get('sample_sheet_input')
-        sample_sheet_name = schema.get('sample_sheet_name', 'samplesheet')
-        header = schema.get('header', 'null')
-
-        # fix rows
-        rows = schema.get('rows')
-        for i, r in enumerate(rows):
-            if "." not in r:
-                if r == 'path':
-                    n = 0
-                    new_r = f'files[{n}].path'
-                    while new_r in rows:
-                        n += 1
-                        new_r = f'files[{n}].path'
-                    rows[i] = new_r
-                else:
-                    rows[i] = f'files[0].metadata.{r}'
-
-        defaults = schema.get('defaults', 'null')
-
-        # fix group by
-        group_by = schema.get('group_by')
-        if type(group_by) is str:
-            group_by = [group_by]
-        for i, gb in enumerate(group_by):
-
-            if "." not in gb:
-                if gb in ['file', 'none']:
-                    group_by[i] = 'file.path'
-                else:
-                    group_by[i] = f'file.metadata.{gb}'
-
-        format_ = schema.get('format_', None)
-
-        if format_ and not sample_sheet_name.endswith(format_):
-            sample_sheet_name += f".{format_}".lower()
-
-        if not format_ and not sample_sheet_name.endswith(['.tsv', '.csv']):
-            raise Exception('Sample sheet format could not be identified. '
-                            'Please specify one of "tsv" or "csv" in the '
-                            'sample sheet schema file.')
-
-        if not format_ and sample_sheet_name.endswith(['.tsv', '.csv']):
-            format_ = sample_sheet_name.split('.').pop().lower()
-
-        if format_.lower() not in ['tsv', 'csv']:
-            raise Exception(f'Unrecognized sample sheet format "{format_}".')
-
-        # Step 1:
-        # add a new input to the pipeline
-        #    - new input must not clash with other inputs by ID
-        # Ensure that the new input is unique
-
-        # Create the sample sheet file array input
-        file_input = self.sb_wrapper.safe_add_input(
-            SAMPLE_SHEET_FILE_ARRAY_INPUT
-        )
-        file_input_id = file_input.get('id')
-
-        # Step 2:
-        # add argument for sample sheet
-        #    - requires: sample sheet input (sample_sheet_input),
-        #                file input (ss_file_input)
-        #    - if the sample sheet is provided on input,
-        #      do not generate a new ss
-        input_changes = {
-            'id': sample_sheet_input,
-            'loadContents': True,
-            'inputBinding': REMOVE_INPUT_KEY
-        }
-
-        prefix = self.sb_wrapper.get_input(
-            sample_sheet_input
-        )['inputBinding']['prefix']
-
-        self.sb_wrapper.update_input(input_changes)
-        self.sb_wrapper.add_argument(
-            {
-                "prefix": prefix,
-                "shellQuote": False,
-                "valueFrom": SAMPLE_SHEET_SWITCH.format(
-                    file_input=f"inputs.{file_input_id}",
-                    sample_sheet=f"inputs.{sample_sheet_input}",
-                    sample_sheet_name=sample_sheet_name,
-                )
-            }
-        )
-
-        # Step 3:
-        # add file requirement
-        #    - requires: sample sheet schema
-        #    - add InitialWorkDirRequirement if there are none
-        #    - if there are, append the entry to listing
-        ss = sample_sheet(
-            file_name=sample_sheet_name,
-            sample_sheet_input=f"inputs.{sample_sheet_input}",
-            format_=format_,
-            input_source=f"inputs.{file_input_id}",
-            header=header,
-            rows=rows,
-            defaults=defaults,
-            group_by=group_by,
-        )
-
-        self.sb_wrapper.add_requirement(ss)
-        self.sb_wrapper.add_requirement(INLINE_JS_REQUIREMENT)
-        self.sb_wrapper.add_requirement(LOAD_LISTING_REQUIREMENT)
-
-    def make_output_type(self, key, output_dict, is_record=False):
-        """
-        This creates an output of specific type based on information provided
-        through output_dict.
-
-        :param key:
-        :param output_dict:
-        :param is_record:
-        :return:
-        """
-
-        converted_cwl_output = dict()
-
-        file_pattern = re.compile(r'.*\.(\w+)$')
-        folder_pattern = re.compile(r'[^.]+$')
-        id_key = 'id'
-
-        if is_record:
-            id_key = 'name'
-
-        name = key
-        if 'display' in output_dict:
-            name = output_dict['display']
-
-        clean_id = re.sub(r'[^a-zA-Z0-9_]', "", name.replace(
-            " ", "_")).lower()
-
-        # Case 1: Output is a Record-type
-        if get_dict_depth(output_dict) > 0:
-            # this is a record, go through the dict_ recursively
-            fields = [self.make_output_type(key, val, is_record=True)
-                      for key, val in output_dict.items()]
-
-            used_field_ids = set()
-
-            for field in fields:
-                base_field_id = field.get('name', 'Output')
-
-                # Since name fields can be the same for multiple inputs,
-                # correct the name if it has already been used.
-                chk_id = base_field_id
-                i = 1
-                if chk_id in used_field_ids:
-                    chk_id = f"{base_field_id}_{i}"
-                    i += 1
-                used_field_ids.add(chk_id)
-
-                field['name'] = chk_id
-
-            converted_cwl_output = {
-                id_key: clean_id,
-                "label": name,
-                "type": [
-                    "null",
-                    {
-                        "type": "record",
-                        "fields": fields,
-                        "name": clean_id
-                    }
-                ]
-            }
-
-        # Case 2: Output is a File type
-        elif re.fullmatch(file_pattern, key):
-            # create a list of files output
-            converted_cwl_output = {
-                id_key: clean_id,
-                "label": name,
-                "type": "File[]?",
-                "outputBinding": {
-                    "glob": key
-                }
-            }
-
-        # Case 3: Output is a folder type
-        elif re.fullmatch(folder_pattern, key):
-            # create a list of directories output
-            converted_cwl_output = {
-                id_key: clean_id,
-                "label": name,
-                "type": "Directory[]?",
-                "outputBinding": {
-                    "glob": key,
-                    "loadListing": "deep_listing"
-                }
-            }
-        return converted_cwl_output
-
-    def parse_output_yml(self, yml_file):
-        """
-        Extracts output information from a YAML file, usually in tower.yml
-        format.
-
-        :param yml_file: path to YAML file.
-        :return: list of outputs in CWL format.
-        """
-        outputs = list()
-        yml_schema = yaml.safe_load(yml_file)
-
-        for key, value in yml_schema.items():
-            # Tower yml file can use "tower" key in the yml file to designate
-            # some configurations tower uses. Since these are not output
-            # definitions, we skip these.
-            if key in SKIP_NEXTFLOW_TOWER_KEYS:
-                continue
-            if key == "reports" and type(value) is dict:
-                temp = value.copy()
-                for k, v in temp.items():
-                    changed_key = f"work/**/{k}"
-                    while "/**/**/" in changed_key:
-                        changed_key = changed_key.replace("/**/**/", "/**/")
-                    value[changed_key] = v
-                    del value[k]
-
-            outputs.append(
-                self.make_output_type(key, value)
-            )
-
-        return outputs
-
-    def dump_sb_wrapper(self, out_format=EXTENSIONS.yaml):
-        """
-        Dump SB wrapper for nextflow workflow to a file
-        """
-        print('Writing sb nextflow schema file...')
-        basename = SB_SCHEMA_DEFAULT_NAME
-        counter = 0
-        sb_wrapper_path = os.path.join(
-            self.workflow_path,
-            f'{basename}.{out_format}'
-        )
-
-        while os.path.exists(sb_wrapper_path):
-            counter += 1
-            sb_wrapper_path = os.path.join(
-                self.workflow_path,
-                f'{basename}.{counter}.{out_format}'
-            )
-
-        print(f"Schema written to file <{sb_wrapper_path}>")
-
-        if out_format in EXTENSIONS.yaml_all:
-            with open(sb_wrapper_path, 'w') as f:
-                yaml.dump(self.sb_wrapper.dump(), f, indent=4, sort_keys=True)
-        elif out_format in EXTENSIONS.json_all:
-            with open(sb_wrapper_path, 'w') as f:
-                json.dump(self.sb_wrapper.dump(), f, indent=4, sort_keys=True)
-
-    def generate_sb_app(
-            self, sb_schema=None, sb_entrypoint='main.nf',
-            executor_version=None, sb_package_id=None, execution_mode=None,
-            sample_sheet_schema=None,
-    ):
-        """
-        Generate an SB app for a nextflow workflow, OR edit the one created and
-        defined by the user
-        """
-
-        if sb_schema:
-            sb_schema_dict = pack(sb_schema)
-            self.sb_wrapper.load(sb_schema_dict)
-
-        else:
-            self.sb_wrapper.cwl_version = 'None'
-            self.sb_wrapper.class_ = 'nextflow'
-
-            self.generate_sb_inputs()
-            self.generate_sb_outputs()
-
-            if sample_sheet_schema:
-                self.parse_sample_sheet_schema(open(sample_sheet_schema))
-
-            self.sb_wrapper.set_app_content(
-                code_package=sb_package_id,
-                entrypoint=sb_entrypoint,
-                executor_version=executor_version,
-            )
-
-            if execution_mode:
-                self.sb_wrapper.add_hint({
-                    'class': 'sbg:NextflowExecutionMode',
-                    'value': execution_mode.value
-                })
-
-            if self.sb_doc:
-                self.sb_wrapper.add_docs(self.sb_doc)
-
 
 def main():
     # CLI parameters
     parser = argparse.ArgumentParser()
     parser.add_argument(
         "--profile", default="default", required=False,
         help="SB platform profile as set in the SB API credentials file.",
@@ -505,37 +85,38 @@
              "If not provided, 'main.nf' will be used if available. "
              "If not available, but a single '*.nf' is located in the "
              "workflow-path will be used. If more than one '*.nf' script is "
              "detected, an error is raised.",
     )
     parser.add_argument(
         "--sb-package-id", required=False,
-        help="Id of an already uploaded package",
+        help="Id of an already uploaded package.",
     )
     parser.add_argument(
         "--sb-doc", required=False,
         help="Path to a doc file for sb app. If not provided, README.md "
              "will be used if available",
     )
     parser.add_argument(
         "--dump-sb-app", action="store_true", required=False,
         help="Dump created sb app to file if true and exit",
     )
-    parser.add_argument(
-        "--no-package", action="store_true", required=False,
-        help="Only provide a sb app schema and a git URL for entrypoint",
-    )
+    # parser.add_argument(
+    #     "--no-package", action="store_true", required=False,
+    #     help="Only provide an sb app schema and a git URL for entrypoint",
+    # )
     parser.add_argument(
         "--executor-version", required=False,
         help="Version of the Nextflow executor to be used with the app.",
     )
     parser.add_argument(
         "--execution-mode", type=ExecMode, choices=list(ExecMode),
         required=False, default=None,
-        help="Execution mode for your application.",
+        help="Execution mode for your application. Can be multi-instance or "
+             "single-instance",
     )
     parser.add_argument(
         "--json", action="store_true", required=False,
         help="Dump sb app schema in JSON format (YAML by default)",
     )
     parser.add_argument(
         "--sb-schema", required=False,
@@ -545,14 +126,26 @@
     parser.add_argument(
         "--revision-note", required=False,
         default=None, type=str,
         help="Revision note to be placed in the CWL schema if the app is "
              "uploaded to the sbg platform.",
     )
     parser.add_argument(
+        "--app-name", required=False,
+        default=None, type=str,
+        help="Name of the app to be shown on the platform.",
+    )
+    parser.add_argument(
+        "--exclude", required=False,
+        default=None, type=str, nargs="+",
+        help=f"Glob patterns you want to exclude from the code package. "
+             f"By default the following patterns are excluded: "
+             f"{DEFAULT_EXCLUDE_PATTERNS}"
+    )
+    parser.add_argument(
         "--sample-sheet-schema", required=False,
         default=None, type=str,
         help="Path to the sample sheet schema yaml. The sample sheet schema "
              "should contain the following keys: 'sample_sheet_input', "
              "'sample_sheet_name', 'header', 'rows', 'defaults', 'group_by', "
              "'format_'"
     )
@@ -562,133 +155,131 @@
              "--workflow-path location",
     )
 
     args = parser.parse_args()
 
     # Preprocess CLI parameter values
     # This stores them into variables that can be updated if --auto is used
-    entrypoint = args.entrypoint or \
-        get_entrypoint(args.workflow_path) or 'main.nf'
+    entrypoint = args.entrypoint or None
     sb_schema = args.sb_schema or None
     executor_version = args.executor_version or None
     execution_mode = args.execution_mode or None
     revision_note = args.revision_note or \
         f"Uploaded using sbpack v{__version__}"
     sample_sheet_schema = args.sample_sheet_schema or None
+    label = args.app_name or None
     dump_sb_app = args.dump_sb_app or False
+    sb_package_id = args.sb_package_id or None
+
+    # Input validation
+    if not dump_sb_app and not args.appid and not args.auto:
+        raise Exception(
+            "The --appid argument is required if "
+            "--dump-sb-app and/or --auto are not used"
+        )
+
+    if sb_schema and execution_mode:
+        logger.warning(
+            "Using --sb-schema option overwrites --execution-mode"
+        )
+
+    if sb_schema and label:
+        logger.warning(
+            "Using --sb-schema option overwrites --app-name"
+        )
+
+    if sb_schema and executor_version:
+        logger.warning(
+            "Using --sb-schema option overwrites --executor-version"
+        )
+
+    if sb_schema and entrypoint:
+        logger.warning(
+            "Using --sb-schema option overwrites --entrypoint"
+        )
 
     sb_doc = None
     if args.sb_doc:
         with open(args.sb_doc, 'r') as f:
             sb_doc = f.read()
     elif get_readme(args.workflow_path):
         with open(get_readme(args.workflow_path), 'r') as f:
             sb_doc = f.read()
 
-    test_sign, test_executor_version = get_executor_version(sb_doc or "")
-    if test_sign and executor_version and "edge" not in executor_version:
-        if test_sign == "=" and version.parse(executor_version) != \
-                version.parse(test_executor_version):
-            logger.warning(
-                f"Provided executor version {executor_version} does not"
-                f" match detected version {test_sign}{test_executor_version}"
-            )
-        if test_sign == ">" and version.parse(executor_version) <= \
-                version.parse(test_executor_version):
-            logger.warning(
-                f"Provided executor version {executor_version} does not"
-                f" match detected version {test_sign}{test_executor_version}"
-            )
-        if test_sign == "<" and version.parse(executor_version) >= \
-                version.parse(test_executor_version):
-            logger.warning(
-                f"Provided executor version {executor_version} does not"
-                f" match detected version {test_sign}{test_executor_version}"
-            )
-        if test_sign == ">=" and version.parse(executor_version) < \
-                version.parse(test_executor_version):
-            logger.warning(
-                f"Provided executor version {executor_version} does not"
-                f" match detected version {test_sign}{test_executor_version}"
-            )
-        if test_sign == "<=" and version.parse(executor_version) > \
-                version.parse(test_executor_version):
-            logger.warning(
-                f"Provided executor version {executor_version} does not"
-                f" match detected version {test_sign}{test_executor_version}"
-            )
-
     if args.auto:
         # This is where the magic happens
         if not sb_schema:
             sb_schema = get_latest_sb_schema(args.workflow_path)
-        # detect nextflow executor version from description
-        executor_version = test_executor_version
+            if sb_schema:
+                logger.info(f'Using sb schema <{sb_schema}>')
 
         # Set execution mode to multi-instance
         if not execution_mode:
             execution_mode = ExecMode.multi
+            logger.info(f'Using execution mode <{execution_mode}>')
 
         # locate sample sheet
         if not sample_sheet_schema:
             sample_sheet_schema = get_sample_sheet_schema(args.workflow_path)
+            if sample_sheet_schema:
+                logger.info(
+                    f'Using sample sheet schema <{sample_sheet_schema}>'
+                )
 
         # if appid is not provided, dump the app
         if not args.appid:
             dump_sb_app = True
-
-    # Input validation
-    if not dump_sb_app:
-        # appid is required
-        if not args.appid:
-            raise Exception(
-                "The --appid argument is required if "
-                "--dump-sb-app is not used"
+            logger.info(
+                f'Appid not provided. App is not going to be uploaded.'
             )
 
     nf_wrapper = SBNextflowWrapper(
         workflow_path=args.workflow_path,
-        sb_doc=sb_doc
+        sb_doc=sb_doc,
+        label=label,
+        entrypoint=entrypoint,
+        executor_version=executor_version,
+        sb_package_id=sb_package_id,
     )
 
     if sb_schema:
         # parse input schema
-        nf_wrapper.generate_sb_app(
-            sb_schema=sb_schema
-        )
+        with open(sb_schema, 'r') as s:
+            schema = yaml.safe_load(s)
+            nf_wrapper.sb_wrapper.load(schema)
     else:
         # build schema
         nf_wrapper.nf_schema_build()
 
         # Create app
         nf_wrapper.generate_sb_app(
-            sb_entrypoint=entrypoint,
-            executor_version=executor_version,
             execution_mode=execution_mode,
             sample_sheet_schema=sample_sheet_schema,
         )
 
     # Install app
     if dump_sb_app:
         # Dump app to local file
         out_format = EXTENSIONS.json if args.json else EXTENSIONS.yaml
         nf_wrapper.dump_sb_wrapper(out_format=out_format)
+
     else:
+        # App should be installed on the platform
         api = lib.get_profile(args.profile)
 
-        sb_package_id = None
-        if args.sb_package_id:
-            sb_package_id = args.sb_package_id
-        elif not args.no_package:
+        # 1. if the code package is not provided on input,
+        # create and upload it
+        if not sb_package_id:
             project_id = '/'.join(args.appid.split('/')[:2])
             sb_package_id = zip_and_push_to_sb(
                 api=api,
                 workflow_path=args.workflow_path,
                 project_id=project_id,
-                folder_name='nextflow_workflows'
+                folder_name='nextflow_workflows',
+                exclude_patterns=args.exclude,
             )
 
         nf_wrapper.sb_wrapper.set_app_content(
             code_package=sb_package_id
         )
 
         nf_wrapper.sb_wrapper.add_revision_note(revision_note)
```

## sbpack/noncwl/utils.py

```diff
@@ -2,213 +2,97 @@
 import time
 import shutil
 import logging
 import json
 import yaml
 import re
 
+from typing import Optional
+import fnmatch
 from sbpack.pack import pack
 from sevenbridges.errors import NotFound
 from sbpack.noncwl.constants import (
     PACKAGE_SIZE_LIMIT,
+    DEFAULT_EXCLUDE_PATTERNS,
+)
+from wrabbit.parser.constants import (
     EXTENSIONS,
-    NF_TO_CWL_PORT_MAP,
-    SB_SCHEMA_DEFAULT_NAME
 )
 
 logger = logging.getLogger(__name__)
 logger.setLevel(logging.INFO)
 
 
-def nf_schema_type_mapper(input_type_string):
-    """
-    Convert nextflow schema input type to CWL
-    """
-    type_ = input_type_string.get('type', 'string')
-    format_ = input_type_string.get('format', '')
-
-    return type_mapper(type_, format_)
-
-
-def nf_to_sb_input_mapper(port_id, port_data, category=None, required=False):
-    """
-    Convert a single input from Nextflow schema to SB schema
-    """
-    sb_input = dict()
-    sb_input['id'] = port_id
-    # # Do not convert outdir
-    # if port_id == 'outdir':
-    #     port_data['format'] = ''
-
-    enum_symbols = port_data.get('enum', [])
-
-    if enum_symbols:
-        sb_input['type'] = enum_type(
-            id_=port_id,
-            symbols=enum_symbols,
-        )
-    else:
-        sb_input['type'] = nf_schema_type_mapper(port_data)
-
-    sb_input['inputBinding'] = {
-        'prefix': f'--{port_id}',
-    }
-
-    if not required:
-        sb_input['type'].append('null')
-
-    if category:
-        sb_input['sbg:category'] = category
-
-    for nf_field, sb_field in NF_TO_CWL_PORT_MAP.items():
-        if nf_field in port_data:
-            value = port_data[nf_field]
-            if value == ":" and nf_field == 'default':
-                # Bug prevents running a task if an input's
-                #  default value is exactly ":". This bug will likely be
-                #  fixed at the time of release of this version.
-                value = " :"
-            sb_input[sb_field] = value
-
-    return sb_input
-
-
-def type_mapper(type_, format_) -> list:
-    if isinstance(type_, str):
-        if type_ == 'string' and 'path' in format_:
-            if format_ == 'file-path':
-                return ['File']
-            if format_ == 'directory-path':
-                return ['Directory']
-            if format_ == 'path':
-                return ['File']
-        if type_ == 'string':
-            return ['string']
-        if type_ == 'integer':
-            return ['int']
-        if type_ == 'number':
-            return ['float']
-        if type_ == 'boolean':
-            return ['boolean']
-        if type_ == 'object':
-            # this should be a record type (dictionary)
-            # it is provided as '{"key1": "value1", "key2": "value2"}'
-            return ['string']
-        return [type_]
-    elif isinstance(type_, list):
-        temp_type_list = []
-        for m in type_:
-            temp_type_list.extend(type_mapper(m, format_))
-        return temp_type_list
-
-
-def enum_type(id_: str, symbols: list) -> list:
-    # This can be generalized so that it encompasses create_profile_enum
-    return [
-        {
-            "type": "enum",
-            "name": id_,
-            "symbols": symbols
-        }
-    ]
-
-
-def create_profile_enum(profiles: list):
-    """
-    If profiles are defined in the config file, this input stores the profiles
-    They are added to the commandline as -profile foo,bar,foobar
-    :param profiles: list of profiles
-    :return: Profiles enum array input
-    """
-    return {
-        "id": "profile",
-        "type": [
-            "null",
-            {
-                "type": "array",
-                "items": {
-                    "type": "enum",
-                    "name": "profile",
-                    "symbols": profiles
-                }
-            }
-        ],
-        "label": "Profiles",
-        "doc": "Select which profile(s) you want to use for task execution.",
-        "inputBinding": {
-            "prefix": "-profile",
-            "itemSeparator": ",",
-            "shellQuote": False,
-        }
-    }
-
-
-def get_dict_depth(dict_, level=0):
-    """
-    Find the depth of the dictionary. Example:
-    {'a': 1} - returns 0;
-    {'a': {'b': 2}} - returns 1...
-
-    :param dict_: input dictionary
-    :param level: depth of the outer dict
-    :return: int
-    """
-    n = level
-    for k, v in dict_.items():
-        if type(v) is dict:
-            lv = get_dict_depth(v, level + 1)
-            if lv > n:
-                n = lv
-    return n
-
-
-def zip_and_push_to_sb(api, workflow_path, project_id, folder_name):
+def zip_and_push_to_sb(
+        api, workflow_path, project_id, folder_name,
+        exclude_patterns: Optional[list] = None
+):
     """
     Create .zip package file. Upload .zip file to the designated folder
     for packages on SevenBridges Platform. Delete local .zip file.
     """
-    zip_path = zip_directory(workflow_path)
+    zip_path = zip_directory(workflow_path, exclude_patterns)
     return push_zip(api, zip_path, project_id, folder_name)
 
 
 def update_timestamp(file_name):
     return re.sub(
         r"(?:\.|)_\d{8}-\d{6}$", "", file_name
     ) + f'_{time.strftime("%Y%m%d-%H%M%S")}'
 
 
-def zip_directory(workflow_path):
+def zip_directory(workflow_path, exclude_patterns: Optional[list] = None):
     """
     This will create a temporary directory that will store all files from the
     original directory, except for the .git hidden directory. This dir
     sometimes collects a large amount of files that will not be used by the
     tool, and can increase the size of the archive up to 10 times.
     """
+    if not exclude_patterns:
+        exclude_patterns = []
 
     intermediary_dir = update_timestamp(os.path.abspath(workflow_path))
     os.mkdir(intermediary_dir)
 
     for root, dirs, files in os.walk(workflow_path):
-        pattern = re.compile(r'(?:^|.*/)\.git(?:$|/.*)')
-        if re.match(pattern, root):
-            continue
-
-        dirs = [d for d in dirs if not re.match(pattern, d)]
         for d in dirs:
             source_file = os.path.join(root, d)
             directory_path = os.path.join(intermediary_dir, os.path.relpath(
                 source_file, workflow_path))
-            if not os.path.exists(directory_path):
-                os.mkdir(directory_path)
+
+            if any([
+                fnmatch.fnmatch(
+                    directory_path, os.path.join(intermediary_dir, pattern)
+                ) for pattern in exclude_patterns + DEFAULT_EXCLUDE_PATTERNS
+            ]):
+                continue
+
+            try:
+                if not os.path.exists(directory_path):
+                    os.mkdir(directory_path)
+            except FileNotFoundError:
+                """Skip folders that cannot be created"""
+                pass
 
         for file in files:
             source_file = os.path.join(root, file)
             dest_file = os.path.join(intermediary_dir, os.path.relpath(
                 source_file, workflow_path))
-            shutil.copy2(source_file, dest_file)
+
+            if any([
+                fnmatch.fnmatch(
+                    dest_file, os.path.join(intermediary_dir, pattern)
+                ) for pattern in exclude_patterns + DEFAULT_EXCLUDE_PATTERNS
+            ]):
+                continue
+
+            try:
+                shutil.copy2(source_file, dest_file)
+            except FileNotFoundError:
+                pass
 
     shutil.make_archive(
         intermediary_dir,
         'zip',
         root_dir=intermediary_dir,
         base_dir='./'
     )
@@ -257,183 +141,15 @@
 
     os.remove(zip_path)
     print(f'Temporary local file {zip_path} deleted.')
 
     return uploaded_file_id
 
 
-def get_readme(path):
-    """
-    Find readme file is there is one in the path folder
-    """
-    for file in os.listdir(path):
-        if file.lower() == 'readme.md':
-            return os.path.join(path, file)
-    return None
-
-
-def get_tower_yml(path):
-    """
-    Find tower.yml file is there is one in the path folder
-    """
-    for file in os.listdir(path):
-        if file.lower() == 'tower.yml':
-            return os.path.join(path, file)
-    return None
-
-
-# Nextflow
-def get_entrypoint(path):
-    """
-    Auto find main.nf or similar file is there is one in the path folder.
-    """
-    possible_paths = []
-    for file in os.listdir(path):
-        if file.lower() == 'main.nf':
-            return file
-
-        if file.lower().endswith('.nf'):
-            possible_paths.append(file)
-
-    if len(possible_paths) > 1:
-        raise Exception(
-            'Detected more than 1 nextflow file in the root of the '
-            'workflow-path. Please use `--entrypoint` to specify which script '
-            'you want to use as the workflow entrypoint')
-    elif len(possible_paths) == 1:
-        return possible_paths.pop()
-    else:
-        return None
-
-
-# Nextflow
-def get_latest_sb_schema(path):
-    """
-    Auto find sb_nextflow_schema file.
-    """
-    possible_paths = []
-    for file in os.listdir(path):
-        result = re.findall(
-            fr"(.*{SB_SCHEMA_DEFAULT_NAME}\.?(\d+)?\.(ya?ml|json))", file
-        )
-        if result:
-            result = result.pop(0)
-            if not result[1]:
-                prep = 0, result[0]
-            else:
-                prep = int(result[1]), result[0]
-            possible_paths.append(prep)
-
-    if possible_paths:
-        latest = sorted(possible_paths).pop()[1]
-        sb_schema_path = os.path.join(path, latest)
-        print(f"Located latest sb_nextflow_schema at <{sb_schema_path}>")
-        return sb_schema_path
-    else:
-        return None
-
-
-def get_executor_version(string):
-    result = re.findall(
-        r"\[Nextflow]\([^(]+(%E2%89%A5|%E2%89%A4|=|>|<)(\d{2}\.\d+\.\d+)[^)]+\)",
-        string
-    )
-    if result:
-        sign, version = result.pop(0)
-        if sign == "%E2%89%A5":
-            sign = ">="
-        elif sign == "%E2%89%A4":
-            sign = "<="
-        elif not sign:
-            sign = "="
-
-        print(f"Identified nextflow executor version requirement {sign} {version}")
-        return sign, version
-    else:
-        return None, None
-
-
-def get_sample_sheet_schema(path):
-    ss_path = os.path.join(path, "samplesheet_schema.yaml")
-
-    if os.path.exists(ss_path):
-        print(f"Located latest sample sheet schema at <{ss_path}>")
-        return ss_path
-    else:
-        return None
-
-
-def get_config_files(path):
-    """
-    Auto find config files.
-    """
-    paths = []
-    for file in os.listdir(path):
-        if file.lower().endswith('.config'):
-            paths.append(os.path.join(path, file))
-    return paths or None
-
-
-def find_config_section(file_path: str, section: str) -> str:
-    section_text = ""
-    found_section = False
-    brackets = 0
-
-    with open(file_path, 'r') as file:
-        for line in file.readlines():
-            if found_section:
-                section_text += line
-                brackets += line.count("{") - line.count("}")
-
-            if brackets < 0:
-                break
-
-            if re.findall(section + r'\s+\{', line):
-                section_text += "{\n"
-                found_section = True
-
-    return section_text
-
-
-def parse_config_file(file_path: str) -> dict:
-    profiles_text = find_config_section(file_path, 'profiles')
-
-    # Extract profiles using regex
-    profiles = {}
-    block_pattern = re.compile(
-        r'\s*(\w+)\s*{([^}]+)}', re.MULTILINE | re.DOTALL
-    )
-    key_val_pattern = re.compile(
-        r'([a-zA-Z._]+)(?:\s+|)=(?:\s+|)([^\s]+)'
-    )
-    include_pattern = re.compile(
-        r'includeConfig\s+[\'\"]([a-zA-Z_.\\/]+)[\'\"]'
-    )
-
-    blocks = re.findall(block_pattern, profiles_text)
-    for name, content in blocks:
-        settings = dict(re.findall(key_val_pattern, content))
-        profiles[name] = settings
-        include_path = re.findall(include_pattern, content)
-        if include_path:
-            profiles[name]['includeConfig'] = include_path
-            include_path = include_path.pop()
-            additional_path = os.path.join(
-                os.path.dirname(file_path), include_path)
-            params_text = find_config_section(additional_path, 'params')
-            params = dict(re.findall(key_val_pattern, params_text))
-            for param, val in params.items():
-                profiles[name][f"params.{param}"] = val
-
-    # return currently returns includeConfig and settings, which are not used
-    # but could be used in the future versions of sbpack
-    return profiles
-
-
-# Deprecated
+# Deprecated - used only in WDL
 def update_schema_code_package(sb_schema, schema_ext, new_code_package):
     """
     Update the package in the sb_schema
     """
 
     sb_schema_dict = pack(sb_schema)
     sb_schema_dict['app_content']['code_package'] = new_code_package
```

## sbpack/noncwl/wdl.py

```diff
@@ -5,24 +5,26 @@
 import argparse
 import logging
 from sbpack.version import __version__
 import re
 from subprocess import check_call
 from sbpack.noncwl.utils import (
     zip_and_push_to_sb,
-    get_readme,
     install_or_upgrade_app,
     update_schema_code_package,
 )
 
 from sbpack.noncwl.constants import (
     GENERIC_FILE_ARRAY_INPUT,
     WRAPPER_REQUIREMENTS,
     GENERIC_WDL_OUTPUT_DIRECTORY,
 )
+from wrabbit.parser.utils import (
+    get_readme
+)
 
 logger = logging.getLogger(__name__)
 logger.setLevel(logging.INFO)
 
 JAVA_EXE = os.getenv('SBPACK_WDL_JAVA_EXE', 'java')
```

## sbpack/noncwl/js_templates/sample_sheet_generator.js

### js-beautify {}

```diff
@@ -11,50 +11,53 @@
                         return 1;
                     }
                 }
                 return 0;
             }
         }
 
-        var input_source = [].concat(inputs. {
+        var input_source = [].concat({
             input_source
         }).sort(compareFiles);
-        if (!input_source.length == 0) {
+        if (input_source.length == 0) {
             {
                 // Return empty file if no input files are given.
                 // Ensures that sample sheet is generated only if there are files to
                 // either:
                 //   - map onto an existing sample sheet, or
                 //   - generate a sample sheet from input file info/metadata
                 return "";
             }
         };
 
-        var sample_sheet_input = inputs. {
+        var sample_sheet_input = {
             sample_sheet_input
         };
 
         var sample_sheet = [];
 
         if (sample_sheet_input) {
             {
                 // If the sample sheet file is given, map inputs to the contents
                 var contents = sample_sheet_input.contents.split("\n");
                 var format_ = sample_sheet_input.nameext.slice(1);
 
                 var split_char = "";
 
-                switch (format_) {
+                if (format_ == 'csv') {
                     {
-                        case 'csv':
-                        split_char = ",";
-                        case 'tsv':
-                        split_char = "\t";
+                        split_char = ',';
                     }
-                };
+                }
+
+                if (format_ == 'tsv') {
+                    {
+                        split_char = '\t';
+                    }
+                }
 
                 for (var i = 0; i < input_source.length; i++) {
                     {
                         var file = input_source[i];
                         for (var row = 0; row < contents.length; row++) {
                             {
                                 var row_data = contents[row].split(split_char);
@@ -75,37 +78,39 @@
                     }
                 }
                 sample_sheet = contents;
             }
         } else {
             {
                 // If the samples are given, create the sample sheet from input data
-                var format_ = {
-                    format_
-                };
+                var format_ = "{format_}";
                 var header = {
                     header
                 };
                 var row = {
                     rows
                 };
                 var defaults = {
                     defaults
                 };
                 var group_by = {
                     group_by
                 };
 
                 var split_char = "";
-                switch (format_) {
+
+                if (format_ == 'csv') {
+                    {
+                        split_char = ',';
+                    }
+                }
+
+                if (format_ == 'tsv') {
                     {
-                        case 'csv':
-                        split_char = ",";
-                        case 'tsv':
-                        split_char = "\t";
+                        split_char = '\t';
                     }
                 }
 
                 if (header) {
                     {
                         sample_sheet.push(header.join(split_char));
                     }
@@ -141,15 +146,15 @@
                             {
                                 defaults.push("");
                             }
                         }
                     }
                 };
 
-                for (k in groups) {
+                for (var k in groups) {
                     {
                         var row_data = [];
                         var files = groups[k];
 
                         files.sort(function(a, b) {
                             {
                                 var name_a = a.basename.toUpperCase();
```

## Comparing `sbpack-2024.2.2rc1.dist-info/LICENSE` & `sbpack-2024.5.7rc1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `sbpack-2024.2.2rc1.dist-info/METADATA` & `sbpack-2024.5.7rc1.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sbpack
-Version: 2024.2.2rc1
+Version: 2024.5.7rc1
 Summary: Command line tool to upload and download CWL to and from SB powered platforms.
 Home-page: UNKNOWN
 Author: Seven Bridges
 Author-email: pavle.marinkovic@velsera.com
 Maintainer: Seven Bridges
 Maintainer-email: pavle.marinkovic@velsera.com
 License: UNKNOWN
@@ -24,14 +24,15 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: ruamel.yaml (>=0.16)
 Requires-Dist: sevenbridges-python (>=2.0)
 Requires-Dist: nf-core (==2.1)
+Requires-Dist: wrabbit (==0.1.1)
 Requires-Dist: cwlformat
 Requires-Dist: packaging
 
 # sbpack
 
 ![](https://github.com/rabix/sbpack/workflows/Tests/badge.svg)
 [![PyPI version](https://badge.fury.io/py/sbpack.svg)](https://pypi.org/project/sbpack/)
```

## Comparing `sbpack-2024.2.2rc1.dist-info/RECORD` & `sbpack-2024.5.7rc1.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 sbpack/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 sbpack/lib.py,sha256=tbLY9To1sp9WnH3bbp50xhA5I1Bfvt15jB6oaXURvtE,5754
 sbpack/pack.py,sha256=gpqWlVqrEwRjQR8InkZJHiIJFU_RezIoXyIY3Igk2b0,13554
 sbpack/schemadef.py,sha256=9UVZNi5nUMJz5ZZM9j4z53X8Svizmc_eUTtl0mTapB8,7929
 sbpack/unpack.py,sha256=amyfuytRxvsz0-RARfP1Hm4tbpmMVCfLSaM8U3woh-o,3064
-sbpack/version.py,sha256=zlTf8rjzS_NLbH-cMoaPdTT_PgChUvB4auDGhp-d8wU,28
-sbpack/noncwl/__init__.py,sha256=Pqgm2f-lVD_zd47j1kztF9YvEGmJnE6gTJpzZh-BrhQ,240
-sbpack/noncwl/constants.py,sha256=g-QOclpn1XI0EW9t7SGgzMGBQYccJ96Tvt4li3nVYPE,3965
+sbpack/version.py,sha256=KkqLQ6LZi4RkcMFwz6ytbvJfDgWp8ACpfA8ucBVtM80,28
+sbpack/noncwl/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+sbpack/noncwl/constants.py,sha256=4-MGip8htmZfN1f9UsdpIT8_vlPv51gP6UHxhI_7sBQ,2247
 sbpack/noncwl/copy.py,sha256=oMAJrGJ6FiU4BF2pyqUOcdTam9Ft64vL8n-ywAKIne8,1591
 sbpack/noncwl/copy_app.py,sha256=HpQp9zcsS0XVUixCP-tUWQloWR-98wgZBi0eqdxkWHI,3755
-sbpack/noncwl/nextflow.py,sha256=_0BHszbWMOjdH_OnZRT_W7rpszw3ot_RmtR1ga70-zU,24043
-sbpack/noncwl/utils.py,sha256=AG-p_VkbjxiWvaUOEGeZvFC3B3adwhZIBjbMqxLYtMY,13423
-sbpack/noncwl/wdl.py,sha256=1cREftnlBqeMHzBHGlnApEtZcq1NTveAfnzBW2uAIMA,10243
+sbpack/noncwl/manifest.py,sha256=hTOXM-YklvxqpqCqi2oIYDB_Js4nTMaKBusuucAvQRQ,9768
+sbpack/noncwl/nextflow.py,sha256=QsPjViTVNMk2MJuAPSNqtLw3_JapjDGv_VkVR5heqiE,9540
+sbpack/noncwl/utils.py,sha256=-iV4IU2ZS1DvHbBLsThAns_L_NfoMyzDXV25KBpW0jA,5456
+sbpack/noncwl/wdl.py,sha256=klZO5y7S3FqyFFLcxQY_9MEqZbtTT7_AU-XkjfvmICE,10279
 sbpack/noncwl/wrapper.py,sha256=-9RMOJOKYj_5n4KfzpE7PS3dU1b57xgvJx8-EyOicfI,6360
 sbpack/noncwl/js/sample_sheet_generator.js,sha256=TbPB-y40UicsyGCQmfalWq03OWN-8s26WnVdCCk0UyM,3667
 sbpack/noncwl/js/sample_sheet_switch.js,sha256=XsrjMymWO07V-Qaewb3bJHoK9RhzjBHP_aj6ljYiruA,197
-sbpack/noncwl/js_templates/sample_sheet_generator.js,sha256=EkN8LPQ4_HucrskcgWy5YWQRcE5vBCggR-mIXE0PvaM,3971
+sbpack/noncwl/js_templates/sample_sheet_generator.js,sha256=FO7uO8RSnfeynhXu8gxLNof0zzDLu_cYOOsbOezEq8E,3946
 sbpack/noncwl/js_templates/sample_sheet_switch.js,sha256=JuGde_APcz1a9oNIFmIXGUHwWwjOxSa_deQlgjaloXs,192
-sbpack-2024.2.2rc1.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-sbpack-2024.2.2rc1.dist-info/METADATA,sha256=ZJOoK2_F_n4JYlCbs4Im9yoEJuFA34jaS9pHA1JRttU,7501
-sbpack-2024.2.2rc1.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-sbpack-2024.2.2rc1.dist-info/entry_points.txt,sha256=Y0GQ-7CPDbYlZXoU-oD_j4UDoVKSE3Esy7MotFo09XA,218
-sbpack-2024.2.2rc1.dist-info/top_level.txt,sha256=jYfNbA_EM0kCUdebAs2xxFukxE1XlzB_BbAr4t25Jmg,7
-sbpack-2024.2.2rc1.dist-info/RECORD,,
+sbpack-2024.5.7rc1.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+sbpack-2024.5.7rc1.dist-info/METADATA,sha256=TkESH3aRGPX2JN8Xzu4dUHNGVRn1bnPzGtDDStMKvB4,7534
+sbpack-2024.5.7rc1.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+sbpack-2024.5.7rc1.dist-info/entry_points.txt,sha256=Iabuge07olzSmWT9h_jsfLybV7DTezK2svTLP5tAlh4,259
+sbpack-2024.5.7rc1.dist-info/top_level.txt,sha256=jYfNbA_EM0kCUdebAs2xxFukxE1XlzB_BbAr4t25Jmg,7
+sbpack-2024.5.7rc1.dist-info/RECORD,,
```

