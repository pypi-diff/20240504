# Comparing `tmp/panpipelines-0.9.9.tar.gz` & `tmp/panpipelines-1.0.0.tar.gz`

## Comparing `panpipelines-0.9.9.tar` & `panpipelines-1.0.0.tar`

### file list

```diff
@@ -1,179 +1,179 @@
--rw-r--r--   0        0        0     1371 2020-02-02 00:00:00.000000 panpipelines-0.9.9/.github/workflows/python-package.yml
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 panpipelines-0.9.9/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0     5401 2020-02-02 00:00:00.000000 panpipelines-0.9.9/PAN250_Deployment/README.md
--rw-r--r--   0        0        0     1037 2020-02-02 00:00:00.000000 panpipelines-0.9.9/PAN250_Deployment/run_pan250.sh
--rw-r--r--   0        0        0     1429 2020-02-02 00:00:00.000000 panpipelines-0.9.9/PAN250_Deployment/atlas/Arterial/README.md
--rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 panpipelines-0.9.9/PAN250_Deployment/atlas/Arterial/res-02_atlas-Arterial_dseg.tsv
--rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 panpipelines-0.9.9/PAN250_Deployment/atlas/Arterial/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-02_atlas-Arterial_dseg.json
--rw-r--r--   0        0        0    37861 2020-02-02 00:00:00.000000 panpipelines-0.9.9/PAN250_Deployment/atlas/Arterial/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-02_atlas-Arterial_dseg.nii.gz
--rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 panpipelines-0.9.9/PAN250_Deployment/atlas/XTRACT/README.md
--rw-r--r--   0        0        0     1325 2020-02-02 00:00:00.000000 panpipelines-0.9.9/PAN250_Deployment/atlas/XTRACT/res-02_atlas-XTRACT_dseg.txt
--rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 panpipelines-0.9.9/PAN250_Deployment/atlas/XTRACT/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-02_atlas-XTRACT_dseg.json
--rw-r--r--   0        0        0    42696 2020-02-02 00:00:00.000000 panpipelines-0.9.9/PAN250_Deployment/atlas/XTRACT/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-02_atlas-XTRACT_dseg.nii.gz
--rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 panpipelines-0.9.9/PAN250_Deployment/batch_scripts/group_template.pbs
--rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 panpipelines-0.9.9/PAN250_Deployment/batch_scripts/participant_template.pbs
--rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 panpipelines-0.9.9/PAN250_Deployment/batch_scripts/headers/slurm_cpu.pbs
--rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 panpipelines-0.9.9/PAN250_Deployment/batch_scripts/headers/slurm_cpu_highpri.pbs
--rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 panpipelines-0.9.9/PAN250_Deployment/batch_scripts/headers/slurm_cpu_highpri_long.pbs
--rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 panpipelines-0.9.9/PAN250_Deployment/batch_scripts/headers/slurm_cpu_highpri_medium.pbs
--rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 panpipelines-0.9.9/PAN250_Deployment/batch_scripts/headers/slurm_cpu_highpri_small.pbs
--rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 panpipelines-0.9.9/PAN250_Deployment/batch_scripts/headers/slurm_cpu_highpri_tiny.pbs
--rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 panpipelines-0.9.9/PAN250_Deployment/batch_scripts/headers/slurm_cpu_highpri_verylong.pbs
--rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 panpipelines-0.9.9/PAN250_Deployment/batch_scripts/headers/slurm_cpu_small.pbs
--rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 panpipelines-0.9.9/PAN250_Deployment/batch_scripts/headers/slurm_cpu_tiny.pbs
--rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 panpipelines-0.9.9/PAN250_Deployment/batch_scripts/headers/slurm_gpu.pbs
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 panpipelines-0.9.9/PAN250_Deployment/config/license.txt
--rw-r--r--   0        0        0    10449 2020-02-02 00:00:00.000000 panpipelines-0.9.9/PAN250_Deployment/config/pan250.config
--rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 panpipelines-0.9.9/PAN250_Deployment/config/pan250_eddyparams.json
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 panpipelines-0.9.9/PAN250_Deployment/config/credentials/credentials.json
--rw-r--r--   0        0        0    10047 2020-02-02 00:00:00.000000 panpipelines-0.9.9/deployment/README.md
--rwxr-xr-x   0        0        0     1471 2020-02-02 00:00:00.000000 panpipelines-0.9.9/deployment/run_pan_slurm.sh
--rw-r--r--   0        0        0     2740 2020-02-02 00:00:00.000000 panpipelines-0.9.9/deployment/atlas/AAL3/AAL3v1_1mm_index.txt
--rw-r--r--   0        0        0     1612 2020-02-02 00:00:00.000000 panpipelines-0.9.9/deployment/atlas/AAL3/README.md
--rw-r--r--   0        0        0     3254 2020-02-02 00:00:00.000000 panpipelines-0.9.9/deployment/atlas/AAL3/res-01_atlas-AAL3_dseg.tsv
--rw-r--r--   0        0        0     3254 2020-02-02 00:00:00.000000 panpipelines-0.9.9/deployment/atlas/AAL3/res-02_atlas-AAL3_dseg.tsv
--rw-r--r--   0        0        0   119500 2020-02-02 00:00:00.000000 panpipelines-0.9.9/deployment/atlas/AAL3/MNI152NLin6Asym/AAL3v1_1mm_MNI152NLin6Asym.nii.gz
--rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 panpipelines-0.9.9/deployment/atlas/AAL3/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-01_atlas-AAL3_dseg.json
--rw-r--r--   0        0        0   119500 2020-02-02 00:00:00.000000 panpipelines-0.9.9/deployment/atlas/AAL3/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-01_atlas-AAL3_dseg.nii.gz
--rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 panpipelines-0.9.9/deployment/atlas/AAL3/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-02_atlas-AAL3_dseg.json
--rw-r--r--   0        0        0    38695 2020-02-02 00:00:00.000000 panpipelines-0.9.9/deployment/atlas/AAL3/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-02_atlas-AAL3_dseg.nii.gz
--rw-r--r--   0        0        0      997 2020-02-02 00:00:00.000000 panpipelines-0.9.9/deployment/atlas/AAL3/MNI152NLin6Asym/Development/convert.sh
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 panpipelines-0.9.9/deployment/atlas/AAL3/MNI152NLin6Asym/Development/eye.mat
--rw-r--r--   0        0        0     2199 2020-02-02 00:00:00.000000 panpipelines-0.9.9/deployment/atlas/AAL3/MNI152NLin6Asym/Development/getTemplate.py
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 panpipelines-0.9.9/deployment/atlas/Arterial/ArterialAtlasLabels.txt
--rw-r--r--   0        0        0     1429 2020-02-02 00:00:00.000000 panpipelines-0.9.9/deployment/atlas/Arterial/README.md
--rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 panpipelines-0.9.9/deployment/atlas/Arterial/res-01_atlas-Arterial_dseg.tsv
--rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 panpipelines-0.9.9/deployment/atlas/Arterial/res-02_atlas-Arterial_dseg.tsv
--rw-r--r--   0        0        0   182712 2020-02-02 00:00:00.000000 panpipelines-0.9.9/deployment/atlas/Arterial/MNI152NLin6Asym/ArterialAtlas_int.nii.gz
--rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 panpipelines-0.9.9/deployment/atlas/Arterial/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-01_atlas-Arterial_dseg.json
--rw-r--r--   0        0        0   182309 2020-02-02 00:00:00.000000 panpipelines-0.9.9/deployment/atlas/Arterial/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-01_atlas-Arterial_dseg.nii.gz
--rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 panpipelines-0.9.9/deployment/atlas/Arterial/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-02_atlas-Arterial_dseg.json
--rw-r--r--   0        0        0    37861 2020-02-02 00:00:00.000000 panpipelines-0.9.9/deployment/atlas/Arterial/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-02_atlas-Arterial_dseg.nii.gz
--rw-r--r--   0        0        0     1436 2020-02-02 00:00:00.000000 panpipelines-0.9.9/deployment/atlas/HARVCORT/HarvardOxford-Cortical_index.txt
--rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 panpipelines-0.9.9/deployment/atlas/HARVCORT/README.md
--rwxr-xr-x   0        0        0   138203 2020-02-02 00:00:00.000000 panpipelines-0.9.9/deployment/atlas/HARVCORT/MNI152NLinAsym/HarvardOxford-cort-maxprob-thr25-1mm.nii.gz
--rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 panpipelines-0.9.9/deployment/atlas/HARVSUBCORT/HarvardOxford-Subcortical_index.txt
--rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 panpipelines-0.9.9/deployment/atlas/HARVSUBCORT/README.md
--rwxr-xr-x   0        0        0   166519 2020-02-02 00:00:00.000000 panpipelines-0.9.9/deployment/atlas/HARVSUBCORT/MNI152NLinAsym/HarvardOxford-sub-maxprob-thr25-1mm.nii.gz
--rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 panpipelines-0.9.9/deployment/atlas/HCPMMP1_FREESURFER/README.md
--rwxr-xr-x   0        0        0    14105 2020-02-02 00:00:00.000000 panpipelines-0.9.9/deployment/atlas/HCPMMP1_FREESURFER/hcpmmp1_ordered.txt
--rwxr-xr-x   0        0        0    12646 2020-02-02 00:00:00.000000 panpipelines-0.9.9/deployment/atlas/HCPMMP1_FREESURFER/hcpmmp1_original.txt
--rw-r--r--   0        0        0  1316983 2020-02-02 00:00:00.000000 panpipelines-0.9.9/deployment/atlas/HCPMMP1_FREESURFER/lh.HCP-MMP1.annot
--rw-r--r--   0        0        0  1316984 2020-02-02 00:00:00.000000 panpipelines-0.9.9/deployment/atlas/HCPMMP1_FREESURFER/rh.HCP-MMP1.annot
--rw-r--r--   0        0        0     1710 2020-02-02 00:00:00.000000 panpipelines-0.9.9/deployment/atlas/JHU/JHU-labels_index.txt
--rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 panpipelines-0.9.9/deployment/atlas/JHU/JHU-tracts_index.txt
--rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 panpipelines-0.9.9/deployment/atlas/JHU/README.md
--rwxr-xr-x   0        0        0    47474 2020-02-02 00:00:00.000000 panpipelines-0.9.9/deployment/atlas/JHU/MNI152NLinAsym/JHU-ICBM-labels-1mm.nii.gz
--rwxr-xr-x   0        0        0    47922 2020-02-02 00:00:00.000000 panpipelines-0.9.9/deployment/atlas/JHU/MNI152NLinAsym/JHU-ICBM-tracts-maxprob-thr25-1mm.nii.gz
--rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 panpipelines-0.9.9/deployment/atlas/XTRACT/README.md
--rw-r--r--   0        0        0     1195 2020-02-02 00:00:00.000000 panpipelines-0.9.9/deployment/atlas/XTRACT/XTRACT_index.txt
--rw-r--r--   0        0        0     1325 2020-02-02 00:00:00.000000 panpipelines-0.9.9/deployment/atlas/XTRACT/res-01_atlas-XTRACT_dseg.txt
--rw-r--r--   0        0        0     1325 2020-02-02 00:00:00.000000 panpipelines-0.9.9/deployment/atlas/XTRACT/res-02_atlas-XTRACT_dseg.txt
--rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 panpipelines-0.9.9/deployment/atlas/XTRACT/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-01_atlas-XTRACT_dseg.json
--rw-r--r--   0        0        0   191828 2020-02-02 00:00:00.000000 panpipelines-0.9.9/deployment/atlas/XTRACT/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-01_atlas-XTRACT_dseg.nii.gz
--rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 panpipelines-0.9.9/deployment/atlas/XTRACT/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-02_atlas-XTRACT_dseg.json
--rw-r--r--   0        0        0    42696 2020-02-02 00:00:00.000000 panpipelines-0.9.9/deployment/atlas/XTRACT/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-02_atlas-XTRACT_dseg.nii.gz
--rw-r--r--   0        0        0   196623 2020-02-02 00:00:00.000000 panpipelines-0.9.9/deployment/atlas/XTRACT/MNI152NLin6Asym/xtract-tract-atlases-maxprob5-1mm.nii.gz
--rwxr-xr-x   0        0        0    89181 2020-02-02 00:00:00.000000 panpipelines-0.9.9/deployment/atlas/freesurfer_atlas/FreeSurferColorLUT.txt
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 panpipelines-0.9.9/deployment/atlas/freesurfer_atlas/README.md
--rwxr-xr-x   0        0        0    10131 2020-02-02 00:00:00.000000 panpipelines-0.9.9/deployment/atlas/freesurfer_atlas/fs_a2009s.txt
--rw-r--r--   0        0        0     6193 2020-02-02 00:00:00.000000 panpipelines-0.9.9/deployment/atlas/freesurfer_atlas/fs_default.txt
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 panpipelines-0.9.9/deployment/atlas/hcpmmp1_subfields_atlas/README.md
--rwxr-xr-x   0        0        0    14879 2020-02-02 00:00:00.000000 panpipelines-0.9.9/deployment/atlas/hcpmmp1_subfields_atlas/hcpmmp1_subfields_ordered.txt
--rwxr-xr-x   0        0        0    13454 2020-02-02 00:00:00.000000 panpipelines-0.9.9/deployment/atlas/hcpmmp1_subfields_atlas/hcpmmp1_subfields_original.txt
--rw-r--r--   0        0        0      848 2020-02-02 00:00:00.000000 panpipelines-0.9.9/deployment/batch_scripts/group_template.pbs
--rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 panpipelines-0.9.9/deployment/batch_scripts/participant_template.pbs
--rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 panpipelines-0.9.9/deployment/batch_scripts/headers/slurm_cpu.pbs
--rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 panpipelines-0.9.9/deployment/batch_scripts/headers/slurm_cpu_fmriprep.pbs
--rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 panpipelines-0.9.9/deployment/batch_scripts/headers/slurm_cpu_highpri.pbs
--rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 panpipelines-0.9.9/deployment/batch_scripts/headers/slurm_cpu_highpri_fmriprep.pbs
--rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 panpipelines-0.9.9/deployment/batch_scripts/headers/slurm_gpu.pbs
--rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 panpipelines-0.9.9/deployment/batch_scripts/headers/slurm_gpu_highpri.pbs
--rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 panpipelines-0.9.9/deployment/batch_scripts/headers/slurm_gpu_windfall.pbs
--rwxr-xr-x   0        0        0      384 2020-02-02 00:00:00.000000 panpipelines-0.9.9/deployment/config/eddy_params.json
--rwxr-xr-x   0        0        0      379 2020-02-02 00:00:00.000000 panpipelines-0.9.9/deployment/config/eddy_params_cpu.json
--rwxr-xr-x   0        0        0      124 2020-02-02 00:00:00.000000 panpipelines-0.9.9/deployment/config/freebash.sh
--rwxr-xr-x   0        0        0       66 2020-02-02 00:00:00.000000 panpipelines-0.9.9/deployment/config/license.txt
--rw-r--r--   0        0        0    23977 2020-02-02 00:00:00.000000 panpipelines-0.9.9/deployment/config/panpipeconfig_expanded_slurm.config
--rw-r--r--   0        0        0    28701 2020-02-02 00:00:00.000000 panpipelines-0.9.9/deployment/config/panpipeconfig_slurm.config
--rwxr-xr-x   0        0        0       59 2020-02-02 00:00:00.000000 panpipelines-0.9.9/deployment/config/credentials/credentials.json
--rwxr-xr-x   0        0        0      215 2020-02-02 00:00:00.000000 panpipelines-0.9.9/example/run_pan_example.sh
--rw-r--r--   0        0        0     3641 2020-02-02 00:00:00.000000 panpipelines-0.9.9/example/config/panpipeconfig_example.config
--rwxr-xr-x   0        0        0       59 2020-02-02 00:00:00.000000 panpipelines-0.9.9/example/config/credentials/credentials_example.json
--rw-r--r--   0        0        0     5085 2020-02-02 00:00:00.000000 panpipelines-0.9.9/src/panpipelines/Factory.py
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 panpipelines-0.9.9/src/panpipelines/__init__.py
--rw-r--r--   0        0        0     5016 2020-02-02 00:00:00.000000 panpipelines-0.9.9/src/panpipelines/group_subjects.py
--rwxr-xr-x   0        0        0    18596 2020-02-02 00:00:00.000000 panpipelines-0.9.9/src/panpipelines/pan_processing.py
--rw-r--r--   0        0        0     9022 2020-02-02 00:00:00.000000 panpipelines-0.9.9/src/panpipelines/single_subject.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 panpipelines-0.9.9/src/panpipelines/version.py
--rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 panpipelines-0.9.9/src/panpipelines/nodes/__init__.py
--rw-r--r--   0        0        0    14132 2020-02-02 00:00:00.000000 panpipelines-0.9.9/src/panpipelines/nodes/antstransform.py
--rw-r--r--   0        0        0     6406 2020-02-02 00:00:00.000000 panpipelines-0.9.9/src/panpipelines/nodes/aslprep.py
--rw-r--r--   0        0        0     5264 2020-02-02 00:00:00.000000 panpipelines-0.9.9/src/panpipelines/nodes/atlascreate.py
--rw-r--r--   0        0        0    22715 2020-02-02 00:00:00.000000 panpipelines-0.9.9/src/panpipelines/nodes/basil.py
--rw-r--r--   0        0        0     7549 2020-02-02 00:00:00.000000 panpipelines-0.9.9/src/panpipelines/nodes/collate_csv_group.py
--rw-r--r--   0        0        0     6288 2020-02-02 00:00:00.000000 panpipelines-0.9.9/src/panpipelines/nodes/collate_csv_single.py
--rw-r--r--   0        0        0     4563 2020-02-02 00:00:00.000000 panpipelines-0.9.9/src/panpipelines/nodes/dummy.py
--rw-r--r--   0        0        0    10177 2020-02-02 00:00:00.000000 panpipelines-0.9.9/src/panpipelines/nodes/fmriprep.py
--rw-r--r--   0        0        0    10720 2020-02-02 00:00:00.000000 panpipelines-0.9.9/src/panpipelines/nodes/freesurfer.py
--rw-r--r--   0        0        0     3495 2020-02-02 00:00:00.000000 panpipelines-0.9.9/src/panpipelines/nodes/fslanat.py
--rw-r--r--   0        0        0     7191 2020-02-02 00:00:00.000000 panpipelines-0.9.9/src/panpipelines/nodes/glm_randomize_group.py
--rw-r--r--   0        0        0     7622 2020-02-02 00:00:00.000000 panpipelines-0.9.9/src/panpipelines/nodes/lst.py
--rw-r--r--   0        0        0     6175 2020-02-02 00:00:00.000000 panpipelines-0.9.9/src/panpipelines/nodes/noddi.py
--rw-r--r--   0        0        0     8370 2020-02-02 00:00:00.000000 panpipelines-0.9.9/src/panpipelines/nodes/parse_textdata.py
--rw-r--r--   0        0        0    27239 2020-02-02 00:00:00.000000 panpipelines-0.9.9/src/panpipelines/nodes/preproc.py
--rw-r--r--   0        0        0     7806 2020-02-02 00:00:00.000000 panpipelines-0.9.9/src/panpipelines/nodes/qsiprep.py
--rw-r--r--   0        0        0    16463 2020-02-02 00:00:00.000000 panpipelines-0.9.9/src/panpipelines/nodes/roi_extract.py
--rw-r--r--   0        0        0     5324 2020-02-02 00:00:00.000000 panpipelines-0.9.9/src/panpipelines/nodes/roi_mean_group.py
--rw-r--r--   0        0        0    11130 2020-02-02 00:00:00.000000 panpipelines-0.9.9/src/panpipelines/nodes/roi_mean_single.py
--rw-r--r--   0        0        0    10201 2020-02-02 00:00:00.000000 panpipelines-0.9.9/src/panpipelines/nodes/tensor.py
--rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 panpipelines-0.9.9/src/panpipelines/pipelines/__init__.py
--rw-r--r--   0        0        0     1195 2020-02-02 00:00:00.000000 panpipelines-0.9.9/src/panpipelines/pipelines/aslprep_panpipeline.py
--rw-r--r--   0        0        0     1186 2020-02-02 00:00:00.000000 panpipelines-0.9.9/src/panpipelines/pipelines/basil_panpipeline.py
--rw-r--r--   0        0        0     1204 2020-02-02 00:00:00.000000 panpipelines-0.9.9/src/panpipelines/pipelines/collatecsv_panpipeline.py
--rw-r--r--   0        0        0     1278 2020-02-02 00:00:00.000000 panpipelines-0.9.9/src/panpipelines/pipelines/collatecsvgroup_panpipeline.py
--rw-r--r--   0        0        0     1194 2020-02-02 00:00:00.000000 panpipelines-0.9.9/src/panpipelines/pipelines/dummy_panpipeline.py
--rw-r--r--   0        0        0     1198 2020-02-02 00:00:00.000000 panpipelines-0.9.9/src/panpipelines/pipelines/fmriprep_panpipeline.py
--rw-r--r--   0        0        0     1205 2020-02-02 00:00:00.000000 panpipelines-0.9.9/src/panpipelines/pipelines/freesurfer_panpipeline.py
--rw-r--r--   0        0        0     1183 2020-02-02 00:00:00.000000 panpipelines-0.9.9/src/panpipelines/pipelines/lst_panpipeline.py
--rw-r--r--   0        0        0     1190 2020-02-02 00:00:00.000000 panpipelines-0.9.9/src/panpipelines/pipelines/noddi_panpipeline.py
--rw-r--r--   0        0        0     3297 2020-02-02 00:00:00.000000 panpipelines-0.9.9/src/panpipelines/pipelines/panpipeline.py
--rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 panpipelines-0.9.9/src/panpipelines/pipelines/preproc_panpipeline.py
--rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 panpipelines-0.9.9/src/panpipelines/pipelines/qsiprep_panpipeline.py
--rw-r--r--   0        0        0     1205 2020-02-02 00:00:00.000000 panpipelines-0.9.9/src/panpipelines/pipelines/roiextract_panpipeline.py
--rw-r--r--   0        0        0     1192 2020-02-02 00:00:00.000000 panpipelines-0.9.9/src/panpipelines/pipelines/tensor_panpipeline.py
--rw-r--r--   0        0        0     1215 2020-02-02 00:00:00.000000 panpipelines-0.9.9/src/panpipelines/pipelines/textmeasures_panpipeline.py
--rw-r--r--   0        0        0     1208 2020-02-02 00:00:00.000000 panpipelines-0.9.9/src/panpipelines/pipelines/volmeasures_panpipeline.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 panpipelines-0.9.9/src/panpipelines/scripts/__init__.py
--rw-r--r--   0        0        0     7141 2020-02-02 00:00:00.000000 panpipelines-0.9.9/src/panpipelines/scripts/aslprep_panscript.py
--rw-r--r--   0        0        0     1772 2020-02-02 00:00:00.000000 panpipelines-0.9.9/src/panpipelines/scripts/fmriprep_panscript.py
--rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 panpipelines-0.9.9/src/panpipelines/scripts/mne_make_surfaces.py
--rw-r--r--   0        0        0      926 2020-02-02 00:00:00.000000 panpipelines-0.9.9/src/panpipelines/scripts/pancontainer_panscript.py
--rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 panpipelines-0.9.9/src/panpipelines/scripts/panscript.py
--rw-r--r--   0        0        0     3513 2020-02-02 00:00:00.000000 panpipelines-0.9.9/src/panpipelines/scripts/sdcflows_fieldmap.py
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 panpipelines-0.9.9/src/panpipelines/utils/__init__.py
--rw-r--r--   0        0        0    31963 2020-02-02 00:00:00.000000 panpipelines-0.9.9/src/panpipelines/utils/transformer.py
--rw-r--r--   0        0        0    74620 2020-02-02 00:00:00.000000 panpipelines-0.9.9/src/panpipelines/utils/util_functions.py
--rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 panpipelines-0.9.9/src/panpipelines/workflows/__init__.py
--rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 panpipelines-0.9.9/src/panpipelines/workflows/aslprep_workflow.py
--rw-r--r--   0        0        0     6185 2020-02-02 00:00:00.000000 panpipelines-0.9.9/src/panpipelines/workflows/basil_workflow.py
--rw-r--r--   0        0        0     1810 2020-02-02 00:00:00.000000 panpipelines-0.9.9/src/panpipelines/workflows/collatecsv_workflow.py
--rw-r--r--   0        0        0     2064 2020-02-02 00:00:00.000000 panpipelines-0.9.9/src/panpipelines/workflows/collatecsvgroup_workflow.py
--rw-r--r--   0        0        0      720 2020-02-02 00:00:00.000000 panpipelines-0.9.9/src/panpipelines/workflows/dummy_workflow.py
--rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 panpipelines-0.9.9/src/panpipelines/workflows/fmriprep_workflow.py
--rw-r--r--   0        0        0      745 2020-02-02 00:00:00.000000 panpipelines-0.9.9/src/panpipelines/workflows/freesurfer_workflow.py
--rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 panpipelines-0.9.9/src/panpipelines/workflows/lst_workflow.py
--rw-r--r--   0        0        0      818 2020-02-02 00:00:00.000000 panpipelines-0.9.9/src/panpipelines/workflows/noddi_workflow.py
--rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 panpipelines-0.9.9/src/panpipelines/workflows/preproc_workflow.py
--rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 panpipelines-0.9.9/src/panpipelines/workflows/qsiprep_workflow.py
--rw-r--r--   0        0        0     7525 2020-02-02 00:00:00.000000 panpipelines-0.9.9/src/panpipelines/workflows/roiextract_workflow.py
--rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 panpipelines-0.9.9/src/panpipelines/workflows/tensor_workflow.py
--rw-r--r--   0        0        0     1499 2020-02-02 00:00:00.000000 panpipelines-0.9.9/src/panpipelines/workflows/textmeasures_workflow.py
--rw-r--r--   0        0        0     4946 2020-02-02 00:00:00.000000 panpipelines-0.9.9/src/panpipelines/workflows/volmeasures_workflow.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 panpipelines-0.9.9/tests/__init__.py
--rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 panpipelines-0.9.9/tests/test_PANFactory.py
--rw-r--r--   0        0        0     3152 2020-02-02 00:00:00.000000 panpipelines-0.9.9/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 panpipelines-0.9.9/LICENSE
--rw-r--r--   0        0        0    12997 2020-02-02 00:00:00.000000 panpipelines-0.9.9/README.md
--rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 panpipelines-0.9.9/pyproject.toml
--rw-r--r--   0        0        0    15188 2020-02-02 00:00:00.000000 panpipelines-0.9.9/PKG-INFO
+-rw-r--r--   0        0        0     1371 2020-02-02 00:00:00.000000 panpipelines-1.0.0/.github/workflows/python-package.yml
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 panpipelines-1.0.0/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0     5401 2020-02-02 00:00:00.000000 panpipelines-1.0.0/PAN250_Deployment/README.md
+-rw-r--r--   0        0        0     1037 2020-02-02 00:00:00.000000 panpipelines-1.0.0/PAN250_Deployment/run_pan250.sh
+-rw-r--r--   0        0        0     1429 2020-02-02 00:00:00.000000 panpipelines-1.0.0/PAN250_Deployment/atlas/Arterial/README.md
+-rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 panpipelines-1.0.0/PAN250_Deployment/atlas/Arterial/res-02_atlas-Arterial_dseg.tsv
+-rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 panpipelines-1.0.0/PAN250_Deployment/atlas/Arterial/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-02_atlas-Arterial_dseg.json
+-rw-r--r--   0        0        0    37861 2020-02-02 00:00:00.000000 panpipelines-1.0.0/PAN250_Deployment/atlas/Arterial/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-02_atlas-Arterial_dseg.nii.gz
+-rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 panpipelines-1.0.0/PAN250_Deployment/atlas/XTRACT/README.md
+-rw-r--r--   0        0        0     1325 2020-02-02 00:00:00.000000 panpipelines-1.0.0/PAN250_Deployment/atlas/XTRACT/res-02_atlas-XTRACT_dseg.txt
+-rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 panpipelines-1.0.0/PAN250_Deployment/atlas/XTRACT/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-02_atlas-XTRACT_dseg.json
+-rw-r--r--   0        0        0    42696 2020-02-02 00:00:00.000000 panpipelines-1.0.0/PAN250_Deployment/atlas/XTRACT/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-02_atlas-XTRACT_dseg.nii.gz
+-rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 panpipelines-1.0.0/PAN250_Deployment/batch_scripts/group_template.pbs
+-rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 panpipelines-1.0.0/PAN250_Deployment/batch_scripts/participant_template.pbs
+-rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 panpipelines-1.0.0/PAN250_Deployment/batch_scripts/headers/slurm_cpu.pbs
+-rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 panpipelines-1.0.0/PAN250_Deployment/batch_scripts/headers/slurm_cpu_highpri.pbs
+-rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 panpipelines-1.0.0/PAN250_Deployment/batch_scripts/headers/slurm_cpu_highpri_long.pbs
+-rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 panpipelines-1.0.0/PAN250_Deployment/batch_scripts/headers/slurm_cpu_highpri_medium.pbs
+-rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 panpipelines-1.0.0/PAN250_Deployment/batch_scripts/headers/slurm_cpu_highpri_small.pbs
+-rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 panpipelines-1.0.0/PAN250_Deployment/batch_scripts/headers/slurm_cpu_highpri_tiny.pbs
+-rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 panpipelines-1.0.0/PAN250_Deployment/batch_scripts/headers/slurm_cpu_highpri_verylong.pbs
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 panpipelines-1.0.0/PAN250_Deployment/batch_scripts/headers/slurm_cpu_small.pbs
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 panpipelines-1.0.0/PAN250_Deployment/batch_scripts/headers/slurm_cpu_tiny.pbs
+-rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 panpipelines-1.0.0/PAN250_Deployment/batch_scripts/headers/slurm_gpu.pbs
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 panpipelines-1.0.0/PAN250_Deployment/config/license.txt
+-rw-r--r--   0        0        0    10449 2020-02-02 00:00:00.000000 panpipelines-1.0.0/PAN250_Deployment/config/pan250.config
+-rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 panpipelines-1.0.0/PAN250_Deployment/config/pan250_eddyparams.json
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 panpipelines-1.0.0/PAN250_Deployment/config/credentials/credentials.json
+-rw-r--r--   0        0        0    10047 2020-02-02 00:00:00.000000 panpipelines-1.0.0/deployment/README.md
+-rwxr-xr-x   0        0        0     1471 2020-02-02 00:00:00.000000 panpipelines-1.0.0/deployment/run_pan_slurm.sh
+-rw-r--r--   0        0        0     2740 2020-02-02 00:00:00.000000 panpipelines-1.0.0/deployment/atlas/AAL3/AAL3v1_1mm_index.txt
+-rw-r--r--   0        0        0     1612 2020-02-02 00:00:00.000000 panpipelines-1.0.0/deployment/atlas/AAL3/README.md
+-rw-r--r--   0        0        0     3254 2020-02-02 00:00:00.000000 panpipelines-1.0.0/deployment/atlas/AAL3/res-01_atlas-AAL3_dseg.tsv
+-rw-r--r--   0        0        0     3254 2020-02-02 00:00:00.000000 panpipelines-1.0.0/deployment/atlas/AAL3/res-02_atlas-AAL3_dseg.tsv
+-rw-r--r--   0        0        0   119500 2020-02-02 00:00:00.000000 panpipelines-1.0.0/deployment/atlas/AAL3/MNI152NLin6Asym/AAL3v1_1mm_MNI152NLin6Asym.nii.gz
+-rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 panpipelines-1.0.0/deployment/atlas/AAL3/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-01_atlas-AAL3_dseg.json
+-rw-r--r--   0        0        0   119500 2020-02-02 00:00:00.000000 panpipelines-1.0.0/deployment/atlas/AAL3/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-01_atlas-AAL3_dseg.nii.gz
+-rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 panpipelines-1.0.0/deployment/atlas/AAL3/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-02_atlas-AAL3_dseg.json
+-rw-r--r--   0        0        0    38695 2020-02-02 00:00:00.000000 panpipelines-1.0.0/deployment/atlas/AAL3/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-02_atlas-AAL3_dseg.nii.gz
+-rw-r--r--   0        0        0      997 2020-02-02 00:00:00.000000 panpipelines-1.0.0/deployment/atlas/AAL3/MNI152NLin6Asym/Development/convert.sh
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 panpipelines-1.0.0/deployment/atlas/AAL3/MNI152NLin6Asym/Development/eye.mat
+-rw-r--r--   0        0        0     2199 2020-02-02 00:00:00.000000 panpipelines-1.0.0/deployment/atlas/AAL3/MNI152NLin6Asym/Development/getTemplate.py
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 panpipelines-1.0.0/deployment/atlas/Arterial/ArterialAtlasLabels.txt
+-rw-r--r--   0        0        0     1429 2020-02-02 00:00:00.000000 panpipelines-1.0.0/deployment/atlas/Arterial/README.md
+-rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 panpipelines-1.0.0/deployment/atlas/Arterial/res-01_atlas-Arterial_dseg.tsv
+-rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 panpipelines-1.0.0/deployment/atlas/Arterial/res-02_atlas-Arterial_dseg.tsv
+-rw-r--r--   0        0        0   182712 2020-02-02 00:00:00.000000 panpipelines-1.0.0/deployment/atlas/Arterial/MNI152NLin6Asym/ArterialAtlas_int.nii.gz
+-rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 panpipelines-1.0.0/deployment/atlas/Arterial/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-01_atlas-Arterial_dseg.json
+-rw-r--r--   0        0        0   182309 2020-02-02 00:00:00.000000 panpipelines-1.0.0/deployment/atlas/Arterial/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-01_atlas-Arterial_dseg.nii.gz
+-rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 panpipelines-1.0.0/deployment/atlas/Arterial/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-02_atlas-Arterial_dseg.json
+-rw-r--r--   0        0        0    37861 2020-02-02 00:00:00.000000 panpipelines-1.0.0/deployment/atlas/Arterial/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-02_atlas-Arterial_dseg.nii.gz
+-rw-r--r--   0        0        0     1436 2020-02-02 00:00:00.000000 panpipelines-1.0.0/deployment/atlas/HARVCORT/HarvardOxford-Cortical_index.txt
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 panpipelines-1.0.0/deployment/atlas/HARVCORT/README.md
+-rwxr-xr-x   0        0        0   138203 2020-02-02 00:00:00.000000 panpipelines-1.0.0/deployment/atlas/HARVCORT/MNI152NLinAsym/HarvardOxford-cort-maxprob-thr25-1mm.nii.gz
+-rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 panpipelines-1.0.0/deployment/atlas/HARVSUBCORT/HarvardOxford-Subcortical_index.txt
+-rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 panpipelines-1.0.0/deployment/atlas/HARVSUBCORT/README.md
+-rwxr-xr-x   0        0        0   166519 2020-02-02 00:00:00.000000 panpipelines-1.0.0/deployment/atlas/HARVSUBCORT/MNI152NLinAsym/HarvardOxford-sub-maxprob-thr25-1mm.nii.gz
+-rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 panpipelines-1.0.0/deployment/atlas/HCPMMP1_FREESURFER/README.md
+-rwxr-xr-x   0        0        0    14105 2020-02-02 00:00:00.000000 panpipelines-1.0.0/deployment/atlas/HCPMMP1_FREESURFER/hcpmmp1_ordered.txt
+-rwxr-xr-x   0        0        0    12646 2020-02-02 00:00:00.000000 panpipelines-1.0.0/deployment/atlas/HCPMMP1_FREESURFER/hcpmmp1_original.txt
+-rw-r--r--   0        0        0  1316983 2020-02-02 00:00:00.000000 panpipelines-1.0.0/deployment/atlas/HCPMMP1_FREESURFER/lh.HCP-MMP1.annot
+-rw-r--r--   0        0        0  1316984 2020-02-02 00:00:00.000000 panpipelines-1.0.0/deployment/atlas/HCPMMP1_FREESURFER/rh.HCP-MMP1.annot
+-rw-r--r--   0        0        0     1710 2020-02-02 00:00:00.000000 panpipelines-1.0.0/deployment/atlas/JHU/JHU-labels_index.txt
+-rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 panpipelines-1.0.0/deployment/atlas/JHU/JHU-tracts_index.txt
+-rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 panpipelines-1.0.0/deployment/atlas/JHU/README.md
+-rwxr-xr-x   0        0        0    47474 2020-02-02 00:00:00.000000 panpipelines-1.0.0/deployment/atlas/JHU/MNI152NLinAsym/JHU-ICBM-labels-1mm.nii.gz
+-rwxr-xr-x   0        0        0    47922 2020-02-02 00:00:00.000000 panpipelines-1.0.0/deployment/atlas/JHU/MNI152NLinAsym/JHU-ICBM-tracts-maxprob-thr25-1mm.nii.gz
+-rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 panpipelines-1.0.0/deployment/atlas/XTRACT/README.md
+-rw-r--r--   0        0        0     1195 2020-02-02 00:00:00.000000 panpipelines-1.0.0/deployment/atlas/XTRACT/XTRACT_index.txt
+-rw-r--r--   0        0        0     1325 2020-02-02 00:00:00.000000 panpipelines-1.0.0/deployment/atlas/XTRACT/res-01_atlas-XTRACT_dseg.txt
+-rw-r--r--   0        0        0     1325 2020-02-02 00:00:00.000000 panpipelines-1.0.0/deployment/atlas/XTRACT/res-02_atlas-XTRACT_dseg.txt
+-rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 panpipelines-1.0.0/deployment/atlas/XTRACT/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-01_atlas-XTRACT_dseg.json
+-rw-r--r--   0        0        0   191828 2020-02-02 00:00:00.000000 panpipelines-1.0.0/deployment/atlas/XTRACT/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-01_atlas-XTRACT_dseg.nii.gz
+-rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 panpipelines-1.0.0/deployment/atlas/XTRACT/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-02_atlas-XTRACT_dseg.json
+-rw-r--r--   0        0        0    42696 2020-02-02 00:00:00.000000 panpipelines-1.0.0/deployment/atlas/XTRACT/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-02_atlas-XTRACT_dseg.nii.gz
+-rw-r--r--   0        0        0   196623 2020-02-02 00:00:00.000000 panpipelines-1.0.0/deployment/atlas/XTRACT/MNI152NLin6Asym/xtract-tract-atlases-maxprob5-1mm.nii.gz
+-rwxr-xr-x   0        0        0    89181 2020-02-02 00:00:00.000000 panpipelines-1.0.0/deployment/atlas/freesurfer_atlas/FreeSurferColorLUT.txt
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 panpipelines-1.0.0/deployment/atlas/freesurfer_atlas/README.md
+-rwxr-xr-x   0        0        0    10131 2020-02-02 00:00:00.000000 panpipelines-1.0.0/deployment/atlas/freesurfer_atlas/fs_a2009s.txt
+-rw-r--r--   0        0        0     6193 2020-02-02 00:00:00.000000 panpipelines-1.0.0/deployment/atlas/freesurfer_atlas/fs_default.txt
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 panpipelines-1.0.0/deployment/atlas/hcpmmp1_subfields_atlas/README.md
+-rwxr-xr-x   0        0        0    14879 2020-02-02 00:00:00.000000 panpipelines-1.0.0/deployment/atlas/hcpmmp1_subfields_atlas/hcpmmp1_subfields_ordered.txt
+-rwxr-xr-x   0        0        0    13454 2020-02-02 00:00:00.000000 panpipelines-1.0.0/deployment/atlas/hcpmmp1_subfields_atlas/hcpmmp1_subfields_original.txt
+-rw-r--r--   0        0        0      848 2020-02-02 00:00:00.000000 panpipelines-1.0.0/deployment/batch_scripts/group_template.pbs
+-rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 panpipelines-1.0.0/deployment/batch_scripts/participant_template.pbs
+-rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 panpipelines-1.0.0/deployment/batch_scripts/headers/slurm_cpu.pbs
+-rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 panpipelines-1.0.0/deployment/batch_scripts/headers/slurm_cpu_fmriprep.pbs
+-rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 panpipelines-1.0.0/deployment/batch_scripts/headers/slurm_cpu_highpri.pbs
+-rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 panpipelines-1.0.0/deployment/batch_scripts/headers/slurm_cpu_highpri_fmriprep.pbs
+-rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 panpipelines-1.0.0/deployment/batch_scripts/headers/slurm_gpu.pbs
+-rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 panpipelines-1.0.0/deployment/batch_scripts/headers/slurm_gpu_highpri.pbs
+-rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 panpipelines-1.0.0/deployment/batch_scripts/headers/slurm_gpu_windfall.pbs
+-rwxr-xr-x   0        0        0      384 2020-02-02 00:00:00.000000 panpipelines-1.0.0/deployment/config/eddy_params.json
+-rwxr-xr-x   0        0        0      379 2020-02-02 00:00:00.000000 panpipelines-1.0.0/deployment/config/eddy_params_cpu.json
+-rwxr-xr-x   0        0        0      124 2020-02-02 00:00:00.000000 panpipelines-1.0.0/deployment/config/freebash.sh
+-rwxr-xr-x   0        0        0       66 2020-02-02 00:00:00.000000 panpipelines-1.0.0/deployment/config/license.txt
+-rw-r--r--   0        0        0    23977 2020-02-02 00:00:00.000000 panpipelines-1.0.0/deployment/config/panpipeconfig_expanded_slurm.config
+-rw-r--r--   0        0        0    28701 2020-02-02 00:00:00.000000 panpipelines-1.0.0/deployment/config/panpipeconfig_slurm.config
+-rwxr-xr-x   0        0        0       59 2020-02-02 00:00:00.000000 panpipelines-1.0.0/deployment/config/credentials/credentials.json
+-rwxr-xr-x   0        0        0      215 2020-02-02 00:00:00.000000 panpipelines-1.0.0/example/run_pan_example.sh
+-rw-r--r--   0        0        0     3641 2020-02-02 00:00:00.000000 panpipelines-1.0.0/example/config/panpipeconfig_example.config
+-rwxr-xr-x   0        0        0       59 2020-02-02 00:00:00.000000 panpipelines-1.0.0/example/config/credentials/credentials_example.json
+-rw-r--r--   0        0        0     5085 2020-02-02 00:00:00.000000 panpipelines-1.0.0/src/panpipelines/Factory.py
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 panpipelines-1.0.0/src/panpipelines/__init__.py
+-rw-r--r--   0        0        0     5016 2020-02-02 00:00:00.000000 panpipelines-1.0.0/src/panpipelines/group_subjects.py
+-rwxr-xr-x   0        0        0    18596 2020-02-02 00:00:00.000000 panpipelines-1.0.0/src/panpipelines/pan_processing.py
+-rw-r--r--   0        0        0     9022 2020-02-02 00:00:00.000000 panpipelines-1.0.0/src/panpipelines/single_subject.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 panpipelines-1.0.0/src/panpipelines/version.py
+-rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 panpipelines-1.0.0/src/panpipelines/nodes/__init__.py
+-rw-r--r--   0        0        0    22370 2020-02-02 00:00:00.000000 panpipelines-1.0.0/src/panpipelines/nodes/antstransform.py
+-rw-r--r--   0        0        0     6328 2020-02-02 00:00:00.000000 panpipelines-1.0.0/src/panpipelines/nodes/aslprep.py
+-rw-r--r--   0        0        0     6123 2020-02-02 00:00:00.000000 panpipelines-1.0.0/src/panpipelines/nodes/atlascreate.py
+-rw-r--r--   0        0        0    32634 2020-02-02 00:00:00.000000 panpipelines-1.0.0/src/panpipelines/nodes/basil.py
+-rw-r--r--   0        0        0     7549 2020-02-02 00:00:00.000000 panpipelines-1.0.0/src/panpipelines/nodes/collate_csv_group.py
+-rw-r--r--   0        0        0     6288 2020-02-02 00:00:00.000000 panpipelines-1.0.0/src/panpipelines/nodes/collate_csv_single.py
+-rw-r--r--   0        0        0     4563 2020-02-02 00:00:00.000000 panpipelines-1.0.0/src/panpipelines/nodes/dummy.py
+-rw-r--r--   0        0        0    10177 2020-02-02 00:00:00.000000 panpipelines-1.0.0/src/panpipelines/nodes/fmriprep.py
+-rw-r--r--   0        0        0    10720 2020-02-02 00:00:00.000000 panpipelines-1.0.0/src/panpipelines/nodes/freesurfer.py
+-rw-r--r--   0        0        0     3495 2020-02-02 00:00:00.000000 panpipelines-1.0.0/src/panpipelines/nodes/fslanat.py
+-rw-r--r--   0        0        0     7191 2020-02-02 00:00:00.000000 panpipelines-1.0.0/src/panpipelines/nodes/glm_randomize_group.py
+-rw-r--r--   0        0        0     7622 2020-02-02 00:00:00.000000 panpipelines-1.0.0/src/panpipelines/nodes/lst.py
+-rw-r--r--   0        0        0     6175 2020-02-02 00:00:00.000000 panpipelines-1.0.0/src/panpipelines/nodes/noddi.py
+-rw-r--r--   0        0        0     8370 2020-02-02 00:00:00.000000 panpipelines-1.0.0/src/panpipelines/nodes/parse_textdata.py
+-rw-r--r--   0        0        0    27631 2020-02-02 00:00:00.000000 panpipelines-1.0.0/src/panpipelines/nodes/preproc.py
+-rw-r--r--   0        0        0     8504 2020-02-02 00:00:00.000000 panpipelines-1.0.0/src/panpipelines/nodes/qsiprep.py
+-rw-r--r--   0        0        0    16667 2020-02-02 00:00:00.000000 panpipelines-1.0.0/src/panpipelines/nodes/roi_extract.py
+-rw-r--r--   0        0        0     5324 2020-02-02 00:00:00.000000 panpipelines-1.0.0/src/panpipelines/nodes/roi_mean_group.py
+-rw-r--r--   0        0        0    11130 2020-02-02 00:00:00.000000 panpipelines-1.0.0/src/panpipelines/nodes/roi_mean_single.py
+-rw-r--r--   0        0        0    10201 2020-02-02 00:00:00.000000 panpipelines-1.0.0/src/panpipelines/nodes/tensor.py
+-rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 panpipelines-1.0.0/src/panpipelines/pipelines/__init__.py
+-rw-r--r--   0        0        0     1195 2020-02-02 00:00:00.000000 panpipelines-1.0.0/src/panpipelines/pipelines/aslprep_panpipeline.py
+-rw-r--r--   0        0        0     1186 2020-02-02 00:00:00.000000 panpipelines-1.0.0/src/panpipelines/pipelines/basil_panpipeline.py
+-rw-r--r--   0        0        0     1204 2020-02-02 00:00:00.000000 panpipelines-1.0.0/src/panpipelines/pipelines/collatecsv_panpipeline.py
+-rw-r--r--   0        0        0     1278 2020-02-02 00:00:00.000000 panpipelines-1.0.0/src/panpipelines/pipelines/collatecsvgroup_panpipeline.py
+-rw-r--r--   0        0        0     1194 2020-02-02 00:00:00.000000 panpipelines-1.0.0/src/panpipelines/pipelines/dummy_panpipeline.py
+-rw-r--r--   0        0        0     1198 2020-02-02 00:00:00.000000 panpipelines-1.0.0/src/panpipelines/pipelines/fmriprep_panpipeline.py
+-rw-r--r--   0        0        0     1205 2020-02-02 00:00:00.000000 panpipelines-1.0.0/src/panpipelines/pipelines/freesurfer_panpipeline.py
+-rw-r--r--   0        0        0     1183 2020-02-02 00:00:00.000000 panpipelines-1.0.0/src/panpipelines/pipelines/lst_panpipeline.py
+-rw-r--r--   0        0        0     1190 2020-02-02 00:00:00.000000 panpipelines-1.0.0/src/panpipelines/pipelines/noddi_panpipeline.py
+-rw-r--r--   0        0        0     3297 2020-02-02 00:00:00.000000 panpipelines-1.0.0/src/panpipelines/pipelines/panpipeline.py
+-rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 panpipelines-1.0.0/src/panpipelines/pipelines/preproc_panpipeline.py
+-rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 panpipelines-1.0.0/src/panpipelines/pipelines/qsiprep_panpipeline.py
+-rw-r--r--   0        0        0     1205 2020-02-02 00:00:00.000000 panpipelines-1.0.0/src/panpipelines/pipelines/roiextract_panpipeline.py
+-rw-r--r--   0        0        0     1192 2020-02-02 00:00:00.000000 panpipelines-1.0.0/src/panpipelines/pipelines/tensor_panpipeline.py
+-rw-r--r--   0        0        0     1215 2020-02-02 00:00:00.000000 panpipelines-1.0.0/src/panpipelines/pipelines/textmeasures_panpipeline.py
+-rw-r--r--   0        0        0     1208 2020-02-02 00:00:00.000000 panpipelines-1.0.0/src/panpipelines/pipelines/volmeasures_panpipeline.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 panpipelines-1.0.0/src/panpipelines/scripts/__init__.py
+-rw-r--r--   0        0        0     7141 2020-02-02 00:00:00.000000 panpipelines-1.0.0/src/panpipelines/scripts/aslprep_panscript.py
+-rw-r--r--   0        0        0     1772 2020-02-02 00:00:00.000000 panpipelines-1.0.0/src/panpipelines/scripts/fmriprep_panscript.py
+-rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 panpipelines-1.0.0/src/panpipelines/scripts/mne_make_surfaces.py
+-rw-r--r--   0        0        0      926 2020-02-02 00:00:00.000000 panpipelines-1.0.0/src/panpipelines/scripts/pancontainer_panscript.py
+-rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 panpipelines-1.0.0/src/panpipelines/scripts/panscript.py
+-rw-r--r--   0        0        0     3617 2020-02-02 00:00:00.000000 panpipelines-1.0.0/src/panpipelines/scripts/sdcflows_fieldmap.py
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 panpipelines-1.0.0/src/panpipelines/utils/__init__.py
+-rw-r--r--   0        0        0    32043 2020-02-02 00:00:00.000000 panpipelines-1.0.0/src/panpipelines/utils/transformer.py
+-rw-r--r--   0        0        0    85984 2020-02-02 00:00:00.000000 panpipelines-1.0.0/src/panpipelines/utils/util_functions.py
+-rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 panpipelines-1.0.0/src/panpipelines/workflows/__init__.py
+-rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 panpipelines-1.0.0/src/panpipelines/workflows/aslprep_workflow.py
+-rw-r--r--   0        0        0     7839 2020-02-02 00:00:00.000000 panpipelines-1.0.0/src/panpipelines/workflows/basil_workflow.py
+-rw-r--r--   0        0        0     1810 2020-02-02 00:00:00.000000 panpipelines-1.0.0/src/panpipelines/workflows/collatecsv_workflow.py
+-rw-r--r--   0        0        0     2064 2020-02-02 00:00:00.000000 panpipelines-1.0.0/src/panpipelines/workflows/collatecsvgroup_workflow.py
+-rw-r--r--   0        0        0      720 2020-02-02 00:00:00.000000 panpipelines-1.0.0/src/panpipelines/workflows/dummy_workflow.py
+-rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 panpipelines-1.0.0/src/panpipelines/workflows/fmriprep_workflow.py
+-rw-r--r--   0        0        0      745 2020-02-02 00:00:00.000000 panpipelines-1.0.0/src/panpipelines/workflows/freesurfer_workflow.py
+-rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 panpipelines-1.0.0/src/panpipelines/workflows/lst_workflow.py
+-rw-r--r--   0        0        0      818 2020-02-02 00:00:00.000000 panpipelines-1.0.0/src/panpipelines/workflows/noddi_workflow.py
+-rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 panpipelines-1.0.0/src/panpipelines/workflows/preproc_workflow.py
+-rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 panpipelines-1.0.0/src/panpipelines/workflows/qsiprep_workflow.py
+-rw-r--r--   0        0        0     9183 2020-02-02 00:00:00.000000 panpipelines-1.0.0/src/panpipelines/workflows/roiextract_workflow.py
+-rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 panpipelines-1.0.0/src/panpipelines/workflows/tensor_workflow.py
+-rw-r--r--   0        0        0     1499 2020-02-02 00:00:00.000000 panpipelines-1.0.0/src/panpipelines/workflows/textmeasures_workflow.py
+-rw-r--r--   0        0        0     4946 2020-02-02 00:00:00.000000 panpipelines-1.0.0/src/panpipelines/workflows/volmeasures_workflow.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 panpipelines-1.0.0/tests/__init__.py
+-rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 panpipelines-1.0.0/tests/test_PANFactory.py
+-rw-r--r--   0        0        0     3152 2020-02-02 00:00:00.000000 panpipelines-1.0.0/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 panpipelines-1.0.0/LICENSE
+-rw-r--r--   0        0        0    12997 2020-02-02 00:00:00.000000 panpipelines-1.0.0/README.md
+-rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 panpipelines-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0    15188 2020-02-02 00:00:00.000000 panpipelines-1.0.0/PKG-INFO
```

### Comparing `panpipelines-0.9.9/.github/workflows/python-package.yml` & `panpipelines-1.0.0/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.9/.github/workflows/python-publish.yml` & `panpipelines-1.0.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.9/PAN250_Deployment/README.md` & `panpipelines-1.0.0/PAN250_Deployment/README.md`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.9/PAN250_Deployment/run_pan250.sh` & `panpipelines-1.0.0/PAN250_Deployment/run_pan250.sh`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.9/PAN250_Deployment/atlas/Arterial/README.md` & `panpipelines-1.0.0/PAN250_Deployment/atlas/Arterial/README.md`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.9/PAN250_Deployment/atlas/Arterial/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-02_atlas-Arterial_dseg.json` & `panpipelines-1.0.0/PAN250_Deployment/atlas/Arterial/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-02_atlas-Arterial_dseg.json`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.9/PAN250_Deployment/atlas/Arterial/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-02_atlas-Arterial_dseg.nii.gz` & `panpipelines-1.0.0/PAN250_Deployment/atlas/Arterial/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-02_atlas-Arterial_dseg.nii.gz`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.9/PAN250_Deployment/atlas/XTRACT/README.md` & `panpipelines-1.0.0/PAN250_Deployment/atlas/XTRACT/README.md`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.9/PAN250_Deployment/atlas/XTRACT/res-02_atlas-XTRACT_dseg.txt` & `panpipelines-1.0.0/PAN250_Deployment/atlas/XTRACT/res-02_atlas-XTRACT_dseg.txt`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.9/PAN250_Deployment/atlas/XTRACT/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-02_atlas-XTRACT_dseg.json` & `panpipelines-1.0.0/PAN250_Deployment/atlas/XTRACT/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-02_atlas-XTRACT_dseg.json`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.9/PAN250_Deployment/atlas/XTRACT/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-02_atlas-XTRACT_dseg.nii.gz` & `panpipelines-1.0.0/PAN250_Deployment/atlas/XTRACT/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-02_atlas-XTRACT_dseg.nii.gz`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.9/PAN250_Deployment/batch_scripts/group_template.pbs` & `panpipelines-1.0.0/PAN250_Deployment/batch_scripts/group_template.pbs`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.9/PAN250_Deployment/batch_scripts/participant_template.pbs` & `panpipelines-1.0.0/PAN250_Deployment/batch_scripts/participant_template.pbs`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.9/PAN250_Deployment/config/pan250.config` & `panpipelines-1.0.0/PAN250_Deployment/config/pan250.config`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.9/deployment/README.md` & `panpipelines-1.0.0/deployment/README.md`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.9/deployment/run_pan_slurm.sh` & `panpipelines-1.0.0/deployment/run_pan_slurm.sh`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.9/deployment/atlas/AAL3/AAL3v1_1mm_index.txt` & `panpipelines-1.0.0/deployment/atlas/AAL3/AAL3v1_1mm_index.txt`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.9/deployment/atlas/AAL3/README.md` & `panpipelines-1.0.0/deployment/atlas/AAL3/README.md`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.9/deployment/atlas/AAL3/res-01_atlas-AAL3_dseg.tsv` & `panpipelines-1.0.0/deployment/atlas/AAL3/res-01_atlas-AAL3_dseg.tsv`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.9/deployment/atlas/AAL3/res-02_atlas-AAL3_dseg.tsv` & `panpipelines-1.0.0/deployment/atlas/AAL3/res-02_atlas-AAL3_dseg.tsv`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.9/deployment/atlas/AAL3/MNI152NLin6Asym/AAL3v1_1mm_MNI152NLin6Asym.nii.gz` & `panpipelines-1.0.0/deployment/atlas/AAL3/MNI152NLin6Asym/AAL3v1_1mm_MNI152NLin6Asym.nii.gz`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.9/deployment/atlas/AAL3/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-01_atlas-AAL3_dseg.json` & `panpipelines-1.0.0/deployment/atlas/AAL3/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-01_atlas-AAL3_dseg.json`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.9/deployment/atlas/AAL3/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-01_atlas-AAL3_dseg.nii.gz` & `panpipelines-1.0.0/deployment/atlas/AAL3/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-01_atlas-AAL3_dseg.nii.gz`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.9/deployment/atlas/AAL3/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-02_atlas-AAL3_dseg.json` & `panpipelines-1.0.0/deployment/atlas/AAL3/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-02_atlas-AAL3_dseg.json`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.9/deployment/atlas/AAL3/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-02_atlas-AAL3_dseg.nii.gz` & `panpipelines-1.0.0/deployment/atlas/AAL3/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-02_atlas-AAL3_dseg.nii.gz`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.9/deployment/atlas/AAL3/MNI152NLin6Asym/Development/convert.sh` & `panpipelines-1.0.0/deployment/atlas/AAL3/MNI152NLin6Asym/Development/convert.sh`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.9/deployment/atlas/AAL3/MNI152NLin6Asym/Development/getTemplate.py` & `panpipelines-1.0.0/deployment/atlas/AAL3/MNI152NLin6Asym/Development/getTemplate.py`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.9/deployment/atlas/Arterial/README.md` & `panpipelines-1.0.0/deployment/atlas/Arterial/README.md`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.9/deployment/atlas/Arterial/MNI152NLin6Asym/ArterialAtlas_int.nii.gz` & `panpipelines-1.0.0/deployment/atlas/Arterial/MNI152NLin6Asym/ArterialAtlas_int.nii.gz`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.9/deployment/atlas/Arterial/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-01_atlas-Arterial_dseg.json` & `panpipelines-1.0.0/deployment/atlas/Arterial/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-01_atlas-Arterial_dseg.json`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.9/deployment/atlas/Arterial/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-01_atlas-Arterial_dseg.nii.gz` & `panpipelines-1.0.0/deployment/atlas/Arterial/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-01_atlas-Arterial_dseg.nii.gz`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.9/deployment/atlas/Arterial/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-02_atlas-Arterial_dseg.json` & `panpipelines-1.0.0/deployment/atlas/Arterial/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-02_atlas-Arterial_dseg.json`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.9/deployment/atlas/Arterial/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-02_atlas-Arterial_dseg.nii.gz` & `panpipelines-1.0.0/deployment/atlas/Arterial/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-02_atlas-Arterial_dseg.nii.gz`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.9/deployment/atlas/HARVCORT/HarvardOxford-Cortical_index.txt` & `panpipelines-1.0.0/deployment/atlas/HARVCORT/HarvardOxford-Cortical_index.txt`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.9/deployment/atlas/HARVCORT/MNI152NLinAsym/HarvardOxford-cort-maxprob-thr25-1mm.nii.gz` & `panpipelines-1.0.0/deployment/atlas/HARVCORT/MNI152NLinAsym/HarvardOxford-cort-maxprob-thr25-1mm.nii.gz`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.9/deployment/atlas/HARVSUBCORT/MNI152NLinAsym/HarvardOxford-sub-maxprob-thr25-1mm.nii.gz` & `panpipelines-1.0.0/deployment/atlas/HARVSUBCORT/MNI152NLinAsym/HarvardOxford-sub-maxprob-thr25-1mm.nii.gz`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.9/deployment/atlas/HCPMMP1_FREESURFER/README.md` & `panpipelines-1.0.0/deployment/atlas/HCPMMP1_FREESURFER/README.md`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.9/deployment/atlas/HCPMMP1_FREESURFER/hcpmmp1_ordered.txt` & `panpipelines-1.0.0/deployment/atlas/HCPMMP1_FREESURFER/hcpmmp1_ordered.txt`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.9/deployment/atlas/HCPMMP1_FREESURFER/hcpmmp1_original.txt` & `panpipelines-1.0.0/deployment/atlas/HCPMMP1_FREESURFER/hcpmmp1_original.txt`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.9/deployment/atlas/HCPMMP1_FREESURFER/lh.HCP-MMP1.annot` & `panpipelines-1.0.0/deployment/atlas/HCPMMP1_FREESURFER/lh.HCP-MMP1.annot`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.9/deployment/atlas/HCPMMP1_FREESURFER/rh.HCP-MMP1.annot` & `panpipelines-1.0.0/deployment/atlas/HCPMMP1_FREESURFER/rh.HCP-MMP1.annot`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.9/deployment/atlas/JHU/JHU-labels_index.txt` & `panpipelines-1.0.0/deployment/atlas/JHU/JHU-labels_index.txt`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.9/deployment/atlas/JHU/JHU-tracts_index.txt` & `panpipelines-1.0.0/deployment/atlas/JHU/JHU-tracts_index.txt`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.9/deployment/atlas/JHU/MNI152NLinAsym/JHU-ICBM-labels-1mm.nii.gz` & `panpipelines-1.0.0/deployment/atlas/JHU/MNI152NLinAsym/JHU-ICBM-labels-1mm.nii.gz`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.9/deployment/atlas/JHU/MNI152NLinAsym/JHU-ICBM-tracts-maxprob-thr25-1mm.nii.gz` & `panpipelines-1.0.0/deployment/atlas/JHU/MNI152NLinAsym/JHU-ICBM-tracts-maxprob-thr25-1mm.nii.gz`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.9/deployment/atlas/XTRACT/README.md` & `panpipelines-1.0.0/deployment/atlas/XTRACT/README.md`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.9/deployment/atlas/XTRACT/XTRACT_index.txt` & `panpipelines-1.0.0/deployment/atlas/XTRACT/XTRACT_index.txt`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.9/deployment/atlas/XTRACT/res-01_atlas-XTRACT_dseg.txt` & `panpipelines-1.0.0/deployment/atlas/XTRACT/res-01_atlas-XTRACT_dseg.txt`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.9/deployment/atlas/XTRACT/res-02_atlas-XTRACT_dseg.txt` & `panpipelines-1.0.0/deployment/atlas/XTRACT/res-02_atlas-XTRACT_dseg.txt`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.9/deployment/atlas/XTRACT/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-01_atlas-XTRACT_dseg.json` & `panpipelines-1.0.0/deployment/atlas/XTRACT/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-01_atlas-XTRACT_dseg.json`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.9/deployment/atlas/XTRACT/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-01_atlas-XTRACT_dseg.nii.gz` & `panpipelines-1.0.0/deployment/atlas/XTRACT/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-01_atlas-XTRACT_dseg.nii.gz`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.9/deployment/atlas/XTRACT/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-02_atlas-XTRACT_dseg.json` & `panpipelines-1.0.0/deployment/atlas/XTRACT/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-02_atlas-XTRACT_dseg.json`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.9/deployment/atlas/XTRACT/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-02_atlas-XTRACT_dseg.nii.gz` & `panpipelines-1.0.0/deployment/atlas/XTRACT/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-02_atlas-XTRACT_dseg.nii.gz`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.9/deployment/atlas/XTRACT/MNI152NLin6Asym/xtract-tract-atlases-maxprob5-1mm.nii.gz` & `panpipelines-1.0.0/deployment/atlas/XTRACT/MNI152NLin6Asym/xtract-tract-atlases-maxprob5-1mm.nii.gz`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.9/deployment/atlas/freesurfer_atlas/FreeSurferColorLUT.txt` & `panpipelines-1.0.0/deployment/atlas/freesurfer_atlas/FreeSurferColorLUT.txt`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.9/deployment/atlas/freesurfer_atlas/fs_a2009s.txt` & `panpipelines-1.0.0/deployment/atlas/freesurfer_atlas/fs_a2009s.txt`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.9/deployment/atlas/freesurfer_atlas/fs_default.txt` & `panpipelines-1.0.0/deployment/atlas/freesurfer_atlas/fs_default.txt`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.9/deployment/atlas/hcpmmp1_subfields_atlas/hcpmmp1_subfields_ordered.txt` & `panpipelines-1.0.0/deployment/atlas/hcpmmp1_subfields_atlas/hcpmmp1_subfields_ordered.txt`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.9/deployment/atlas/hcpmmp1_subfields_atlas/hcpmmp1_subfields_original.txt` & `panpipelines-1.0.0/deployment/atlas/hcpmmp1_subfields_atlas/hcpmmp1_subfields_original.txt`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.9/deployment/batch_scripts/group_template.pbs` & `panpipelines-1.0.0/deployment/batch_scripts/group_template.pbs`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.9/deployment/batch_scripts/participant_template.pbs` & `panpipelines-1.0.0/deployment/batch_scripts/participant_template.pbs`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.9/deployment/config/panpipeconfig_expanded_slurm.config` & `panpipelines-1.0.0/deployment/config/panpipeconfig_expanded_slurm.config`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.9/deployment/config/panpipeconfig_slurm.config` & `panpipelines-1.0.0/deployment/config/panpipeconfig_slurm.config`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.9/example/config/panpipeconfig_example.config` & `panpipelines-1.0.0/example/config/panpipeconfig_example.config`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.9/src/panpipelines/Factory.py` & `panpipelines-1.0.0/src/panpipelines/Factory.py`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.9/src/panpipelines/group_subjects.py` & `panpipelines-1.0.0/src/panpipelines/group_subjects.py`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.9/src/panpipelines/pan_processing.py` & `panpipelines-1.0.0/src/panpipelines/pan_processing.py`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.9/src/panpipelines/single_subject.py` & `panpipelines-1.0.0/src/panpipelines/single_subject.py`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.9/src/panpipelines/nodes/aslprep.py` & `panpipelines-1.0.0/src/panpipelines/nodes/aslprep.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,15 +36,14 @@
     aslprep_dict = updateParams(aslprep_dict,"--participant_label","<PARTICIPANT_LABEL>")
     aslprep_dict = updateParams(aslprep_dict,"--low-mem",IS_PRESENT)
     aslprep_dict = updateParams(aslprep_dict,"--skip-bids-validation",IS_PRESENT)
     aslprep_dict = updateParams(aslprep_dict,"--stop-on-first-crash",IS_PRESENT)
     aslprep_dict = updateParams(aslprep_dict,"--mem_mb","<BIDSAPP_MEMORY>")
     aslprep_dict = updateParams(aslprep_dict,"--nthreads","<BIDSAPP_THREADS>")
     aslprep_dict = updateParams(aslprep_dict,"--fs-license-file","<FSLICENSE>")
-    aslprep_dict = updateParams(aslprep_dict,"--ignore fieldmaps",IS_PRESENT)
     aslprep_dict = updateParams(aslprep_dict,"-w","<CWD>/aslprep_work")
 
     # Additional params
     ASLPREP_OVERRIDE_PARAMS = getParams(labels_dict,"ASLPREP_OVERRIDE_PARAMS")
     if ASLPREP_OVERRIDE_PARAMS and isinstance(ASLPREP_OVERRIDE_PARAMS,dict):
         add_labels(ASLPREP_OVERRIDE_PARAMS,aslprep_dict)
```

### Comparing `panpipelines-0.9.9/src/panpipelines/nodes/atlascreate.py` & `panpipelines-1.0.0/src/panpipelines/nodes/atlascreate.py`

 * *Files 9% similar despite different names*

```diff
@@ -12,51 +12,69 @@
 def atlascreate_proc(labels_dict,roi_list,roilabels_list):
 
     cwd=os.getcwd()
     labels_dict = updateParams(labels_dict,"CWD",cwd)
     output_dir = cwd
  
     participant_label = getParams(labels_dict,'PARTICIPANT_LABEL')
+    participant_session = getParams(labels_dict,'PARTICIPANT_SESSION')
 
-    atlas_name = getParams(labels_dict,'ATLAS_NAME')
+    atlas_name = getParams(labels_dict,'NEWATLAS_NAME')
     atlas_workdir = os.path.join(cwd,'{}_workdir'.format(atlas_name))
     if not os.path.isdir(atlas_workdir):
         os.makedirs(atlas_workdir)
 
-    atlas_file = newfile(cwd, atlas_name, prefix=f"sub-{participant_label}", extension="nii.gz")
+    atlas_file = newfile(cwd, atlas_name, prefix=f"sub-{participant_label}_ses-{participant_session}", extension="nii.gz")
     IFLOGGER.info(f"Creating new atlas {atlas_file}")
 
     special_atlas_type=""
     # scan through the roi list and find out if we have a special atlas type
     if roi_list[0] == "hcpmmp1aseg":
         special_atlas_type="hcpmmp1aseg"
 
 
     atlas_type = "3D"
     atlas_type = getParams(labels_dict,'NEWATLAS_TYPE')
 
+    prob_thresh =  getParams(labels_dict,'NEWATLAS_PROBTHRESH')
+    if prob_thresh:
+        if not isinstance(prob_thresh,list):
+            prob_thresh = float(prob_thresh)
+    else:
+        prob_thresh = 0.5
+
+    invert_roi =  getParams(labels_dict,'NEWATLAS_INVERTROI')
+    if invert_roi:
+        if not isinstance(invert_roi,list):
+            invert_roi = isTrue(invert_roi)
+    else:
+        invert_roi = False
+
     atlas_index_mode = None
     if getParams(labels_dict,'NEWATLAS_INDEX_MODE'):
         atlas_index_mode = getParams(labels_dict,'NEWATLAS_INDEX_MODE')
     elif getParams(labels_dict,'ATLAS_INDEX_MODE'):
         atlas_index_mode = getParams(labels_dict,'ATLAS_INDEX_MODE')
 
     if special_atlas_type == "hcpmmp1aseg":
         roilabels_list=create_3d_hcpmmp1_aseg(atlas_file,roi_list,labels_dict)
         if not atlas_index_mode:
             atlas_index_mode = "hcpmmp1aseg_tsv"
         roi_list = [atlas_file]
     elif atlas_type == "3D":
-        create_3d_atlas_from_rois(atlas_file, roi_list,labels_dict)
+        create_3d_atlas_from_rois(atlas_file, roi_list,labels_dict,prob_thresh=prob_thresh)
     elif atlas_type == "3D_contig":
-        create_3d_atlas_from_rois(atlas_file, roi_list,labels_dict,explode3d=False)
+        create_3d_atlas_from_rois(atlas_file, roi_list,labels_dict,prob_thresh=prob_thresh,explode3d=False)
+    elif atlas_type == "3D_mask":
+        roi_values = getParams(labels_dict,'MASK_ROIVALUE')
+        create_3d_mask_from_rois(atlas_file, roi_list,labels_dict,roi_values=roi_values, prob_thresh=prob_thresh,explode3d=False,invert_roi=invert_roi)
     elif atlas_type =="4D":
-        create_4d_atlas_from_rois(atlas_file, roi_list,labels_dict)
+        create_4d_atlas_from_rois(atlas_file, roi_list,labels_dict,low_thresh=prob_thresh)
     else:
-        create_3d_atlas_from_rois(atlas_file, roi_list,labels_dict)
+        create_3d_atlas_from_rois(atlas_file, roi_list,labels_dict,prob_thresh=prob_thresh)
 
     if not atlas_index_mode:
         atlas_index_mode = "tsv"
 
     if "tsv" in atlas_index_mode:
         atlas_index = newfile(cwd, atlas_name, prefix=f"sub-{participant_label}", suffix="dseg",extension="tsv")
     else:
```

### Comparing `panpipelines-0.9.9/src/panpipelines/nodes/collate_csv_group.py` & `panpipelines-1.0.0/src/panpipelines/nodes/collate_csv_group.py`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.9/src/panpipelines/nodes/collate_csv_single.py` & `panpipelines-1.0.0/src/panpipelines/nodes/collate_csv_single.py`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.9/src/panpipelines/nodes/dummy.py` & `panpipelines-1.0.0/src/panpipelines/nodes/dummy.py`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.9/src/panpipelines/nodes/fmriprep.py` & `panpipelines-1.0.0/src/panpipelines/nodes/fmriprep.py`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.9/src/panpipelines/nodes/freesurfer.py` & `panpipelines-1.0.0/src/panpipelines/nodes/freesurfer.py`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.9/src/panpipelines/nodes/fslanat.py` & `panpipelines-1.0.0/src/panpipelines/nodes/fslanat.py`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.9/src/panpipelines/nodes/glm_randomize_group.py` & `panpipelines-1.0.0/src/panpipelines/nodes/glm_randomize_group.py`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.9/src/panpipelines/nodes/lst.py` & `panpipelines-1.0.0/src/panpipelines/nodes/lst.py`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.9/src/panpipelines/nodes/noddi.py` & `panpipelines-1.0.0/src/panpipelines/nodes/noddi.py`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.9/src/panpipelines/nodes/parse_textdata.py` & `panpipelines-1.0.0/src/panpipelines/nodes/parse_textdata.py`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.9/src/panpipelines/nodes/preproc.py` & `panpipelines-1.0.0/src/panpipelines/nodes/preproc.py`

 * *Files 4% similar despite different names*

```diff
@@ -109,14 +109,20 @@
     npzero3d = np.zeros((dimN,dimN,dimN))
     disc2d = getDisc(dimN,dimN)
     for dimz in range(dimN):
         npzero3d[:,:,dimz] = np.multiply(np.multiply(np.ones((dimN,dimN)),disc2d[dimz,:]),disc2d[dimz,:].reshape(-1,1))
 
     return npzero3d
 
+def within_range(vox,dims):
+    if vox[0] > (dims[0] - 1) or vox[1] > (dims[1] - 1) or  vox[2] > (dims[2] - 1):
+        return False
+    
+    return True
+
 def derive_asl_artefact_v2(asl_acq,labels_dict,command_base,participant_label,participant_session,artefact_outputdir,PHASESHIFT=12,PHASEAXIS=1,ALLOWOVERLAP=False,CLOSE_DISC_STR="",DILATE_DISC_STR="disc-1",ERODE_DISC_STR="",T1_DILATE_DISC_STR="",COMBINED_ERODE_DISC_STR="",FILL_HOLES_STR="2",expand_ring=["1","1"],DO_T1_SHIFT=True, DO_CONSERVATIVE=True):
 
 
     transform_list =  getParams(labels_dict,'TRANSFORM_MAT')
     transform_ref =  getParams(labels_dict,'TRANSFORM_REF')
     PHASESHIFT_lookup = getParams(labels_dict,'PHASESHIFT')
     if PHASESHIFT_lookup:
@@ -160,18 +166,22 @@
     # set up dwi to process just the specific dwi session
     subject = f"sub-{participant_label}"
     if participant_session:
         session = f"ses-{participant_session}"
     else:
         session=""
 
+    artefact_subdirname="asl_artefact"
+    if getParams(labels_dict,'CHEMSHIFT_DIRNAME'):
+        artefact_subdirname = getParams(labels_dict,'CHEMSHIFT_DIRNAME')
+
     if not artefact_outputdir:
-        artefact_outputdir = os.path.join(output_dir,"asl_artefact", subject,session)
+        artefact_outputdir = os.path.join(output_dir,artefact_subdirname, subject,session)
     else:
-        artefact_outputdir = os.path.join(artefact_outputdir,"asl_artefact", subject,session)
+        artefact_outputdir = os.path.join(artefact_outputdir,artefact_subdirname, subject,session)
 
     if not os.path.exists(artefact_outputdir):
         os.makedirs(artefact_outputdir, exist_ok=True)
 
 
     subjects_dir = getParams(labels_dict,'SUBJECTS_DIR')
     outer_skull=os.path.join(subjects_dir,subject,'bem','outer_skull.surf')
@@ -195,27 +205,33 @@
     origimg_shape = origimg.shape
     outer_skull_vol = np.zeros((origimg_shape),dtype=origimg_dtype)
     inv_Torig = npl.inv(Torig)
 
     for rr in rr_mm_outer_skull:
         vox = apply_affine(inv_Torig, rr)
         vox_ind = tuple(np.round(vox).astype(int))
-        outer_skull_vol[vox_ind] = 255
+        if within_range(vox_ind,origimg_shape):
+            outer_skull_vol[vox_ind] = 255
+        else:
+            IFLOGGER.warn(f"{vox} outside range of {origimg_shape} for surface {rr}")
 
     for tri in tris_outer_skull:
         p0 = np.round(apply_affine(inv_Torig,rr_mm_outer_skull[tri[0]])).astype(int)
         p1 = np.round(apply_affine(inv_Torig,rr_mm_outer_skull[tri[1]])).astype(int)
         p2 = np.round(apply_affine(inv_Torig,rr_mm_outer_skull[tri[2]])).astype(int)
         if DO_CONSERVATIVE:
             valid_vox = returnCandidatesConservative(p0,p1,p2)
         else:
             valid_vox = returnCandidates(p0,p1,p2)
         for vox in valid_vox:
             vox_ind = tuple(vox.astype(int))
-            outer_skull_vol[vox_ind] = 255
+            if within_range(vox_ind,origimg_shape):
+                outer_skull_vol[vox_ind] = 255
+            else:
+                IFLOGGER.warn(f"{vox} outside range of {origimg_shape} for surface {rr}")
     outer_skull_img = nibabel.Nifti1Image(outer_skull_vol,origimg.affine,origimg.header)
     outer_skull_img_file=os.path.join(work_dir,f"{subject}_{session}_outer_skull.nii.gz")
     nibabel.save(outer_skull_img,outer_skull_img_file) 
 
     if T1_DILATE_DISC_STR:
         T1_DILATE_DISC=int(T1_DILATE_DISC_STR.split("-")[1])
         STREL_TYPE=T1_DILATE_DISC_STR.split("-")[0]
@@ -399,15 +415,15 @@
             else:
                 print(f"phase axis {PHASEAXIS} not valid. Allowing overlap of mask")     
         shifted_img = nibabel.Nifti1Image(data_shifted,outskull_aslspace_img.affine,outskull_aslspace_img.header)
         nibabel.save(shifted_img,outer_skull_shift)
         outer_skull_shifted_images.append(outer_skull_shift)
 
     if len(outer_skull_shifted_images) > 1:
-        command = f"fslmaths {outer_skull_shifted_images[0]} "
+        command = f"{command_base} fslmaths {outer_skull_shifted_images[0]} "
         for shifted_image in outer_skull_shifted_images[1:]:
             command = command + f"-add {shifted_image} "
 
         outer_skull_shift_combined=newfile(work_dir,outer_skull_shift,suffix=f"combined")
         command = command + f"-bin {outer_skull_shift_combined} "
         evaluated_command=substitute_labels(command, labels_dict)
         results = runCommand(evaluated_command,IFLOGGER)
@@ -567,20 +583,16 @@
             asl_acq = get_bidstag("acq",asl_bidsfile.filename)
 
         if not asl_acq:
             asl_acq = "default"
 
         artefact_outputdir = getParams(labels_dict,'DERIVATIVES_DIR')
         if not artefact_outputdir:
-            artefact_outputdir = os.path.join(output_dir,"asl_artefact", subject,session)
-        else:
-            artefact_outputdir = os.path.join(artefact_outputdir,"asl_artefact", subject,session)
+            artefact_outputdir = output_dir
 
-        if not os.path.exists(artefact_outputdir):
-            os.makedirs(artefact_outputdir, exist_ok=True)
 
         if VERSION_TO_RUN == "2":
             derive_asl_artefact_v2(asl_acq,labels_dict,command_base, participant_label,participant_session,artefact_outputdir)
         else:
             m0_entities = asl_entities.copy()
             m0_entities["suffix"]="m0scan"
             m0  = layout.get(return_type='file', invalid_filters='allow', **m0_entities)
```

### Comparing `panpipelines-0.9.9/src/panpipelines/nodes/qsiprep.py` & `panpipelines-1.0.0/src/panpipelines/nodes/qsiprep.py`

 * *Files 5% similar despite different names*

```diff
@@ -47,14 +47,23 @@
 
     if eddy_json and eddy_update and isinstance(eddy_update,dict):
         for itemkey,itemvalue in eddy_update.items():
             eddy_json[itemkey] = substitute_labels(itemvalue,labels_dict)
         eddy_config = newfile(cwd,eddy_config,prefix=f"sub-{participant_label}_ses-{participant_session}")
         export_labels(eddy_json, eddy_config)
 
+    unique_eddy_update = getParams(labels_dict,'UNIQUE_EDDY_CONFIG_UPDATE')
+    if eddy_json and unique_eddy_update and isinstance(unique_eddy_update,dict):
+        for itemkey,itemvalue in unique_eddy_update.items():
+            if itemkey == f"{participant_label}_{participant_session}" or itemkey == f"{participant_label}" and isinstance(itemvalue,dict):
+                for subitemkey,subitemvalue in itemvalue.items():
+                    eddy_json[subitemkey] = substitute_labels(subitemvalue,labels_dict)
+                eddy_config = newfile(cwd,eddy_config,prefix=f"sub-{participant_label}_ses-{participant_session}",suffix="unique")
+                export_labels(eddy_json, eddy_config)
+
     # This is for 1 specific scenario - we will terminate early if field map is missing
     layout = BIDSLayout(bids_dir)
     epi = layout.get(subject=participant_label, session=participant_session, suffix="epi",extension=".nii.gz") 
     if not epi:
         IFLOGGER.warn(f"Fieldmap not found for subject {participant_label} and session {participant_session}. terminating script early.")
         sys.exit(1)
```

### Comparing `panpipelines-0.9.9/src/panpipelines/nodes/roi_extract.py` & `panpipelines-1.0.0/src/panpipelines/nodes/roi_extract.py`

 * *Files 9% similar despite different names*

```diff
@@ -14,30 +14,41 @@
 from nipype import logging as nlogging
 from nilearn.maskers import NiftiLabelsMasker
 from nilearn.maskers import NiftiMapsMasker
 from nilearn import image
 
 IFLOGGER=nlogging.getLogger('nipype.interface')
 
-def roi_extract_proc(labels_dict,input_file,atlas_file,atlas_index, lesion_file):
+def roi_extract_proc(labels_dict,input_file,atlas_file,atlas_index, mask_file):
 
     metadata_comments=""
     cwd=os.getcwd()
     labels_dict = updateParams(labels_dict,"CWD",cwd)
     output_dir=cwd
     participant_label = getParams(labels_dict,'PARTICIPANT_LABEL')
     session_label = getParams(labels_dict,'PARTICIPANT_SESSION')
 
-    lesion_inverse_img = None
-    if lesion_file and not lesion_file == ".": 
-        lesion_img = nib.load(lesion_file)
-        lesion_data = lesion_img.get_fdata()
-        inverse_data = np.zeros(lesion_data.shape)
-        inverse_data[lesion_data < 1] = 1 
-        lesion_inverse_img=nib.Nifti1Image(inverse_data, lesion_img.affine)
+    INVERT_MASK = isTrue(getParams(labels_dict,'MASK_INVERT'))
+    MASK_NAME = getParams(labels_dict,'MASK_NAME')
+    if not MASK_NAME:
+        MASK_NAME = "mask"
+
+    mask_img =None
+    mask_inverse_img = None
+    if mask_file and not mask_file == ".": 
+        IFLOGGER.info(f"{mask_file} provided to mask measures.")
+        mask_img = nib.load(mask_file)
+        mask_data = mask_img.get_fdata()
+        if INVERT_MASK:
+            IFLOGGER.info(f"Inverse of {mask_file} will be used to mask results.")
+            inverse_data = np.zeros(mask_data.shape)
+            inverse_data[mask_data < 1] = 1 
+            mask_inverse_img=nib.Nifti1Image(inverse_data, mask_img.affine)
+        else:
+            mask_inverse_img=mask_img
 
     
     if not session_label:
         roi_output_dir = os.path.join(cwd,f"sub-{participant_label}_roi_output_dir")
     else:
         roi_output_dir = os.path.join(cwd,f"sub-{participant_label}_ses-{session_label}_roi_output_dir")
 
@@ -60,24 +71,14 @@
             os.makedirs(mgzdir)
 
         fs_command_base, fscontainer = getContainer(labels_dict,nodename="convMGZ2NII",SPECIFIC="FREESURFER_CONTAINER",LOGGER=IFLOGGER)
         input_file_nii = newfile(mgzdir,input_file,extension=".nii.gz")
         convMGZ2NII(input_file, input_file_nii, fs_command_base)
         input_file = input_file_nii
 
-    if Path(lesion_file).suffix == ".mgz":
-        mgzdir = os.path.join(cwd,'mgz_nii')
-        if not os.path.isdir(mgzdir):
-            os.makedirs(mgzdir)
-
-        fs_command_base, fscontainer = getContainer(labels_dict,nodename="convMGZ2NII",SPECIFIC="FREESURFER_CONTAINER",LOGGER=IFLOGGER)
-        lesion_file_nii = newfile(mgzdir,lesion_file,extension=".nii.gz")
-        convMGZ2NII(lesion_file, lesion_file_nii, fs_command_base)
-        lesion_file = lesion_file_nii
-
     atlas_type="3D"
     atlas_img  = nib.load(atlas_file)
     atlas_dim = 1
     atlas_shape = atlas_img.header.get_data_shape()
     if len(atlas_shape) > 3:
         if atlas_shape[3]> 1:
             atlas_type="4D"
@@ -123,42 +124,47 @@
     measure_data = measure_img.get_fdata()
     measure_shape = measure_img.header.get_data_shape()
     if len(measure_shape) > 3:
         if measure_shape[3] > 1:
             measure_type = "4D"
 
     if atlas_type == "4D":
-        if lesion_inverse_img:
+        if mask_inverse_img:
             NiftiMasker = NiftiMapsMasker(
                 atlas_img,
-                mask_img = lesion_inverse_img,
+                mask_img = mask_inverse_img,
                 Labels = labels_name_list,
                 standardize=False
             )
         else:
             NiftiMasker = NiftiMapsMasker(
                 atlas_img,
                 Labels = labels_name_list,
                 standardize=False
             )
     else:
-        if lesion_inverse_img:
+        if mask_inverse_img:
             NiftiMasker = NiftiLabelsMasker(
                 atlas_img,
-                mask_img = lesion_inverse_img,
+                mask_img = mask_inverse_img,
                 Labels = labels_name_list,
                 standardize=False
             )
         else:
             NiftiMasker = NiftiLabelsMasker(
                 atlas_img,
                 Labels = labels_name_list,
                 standardize=False
             )
 
+    mask_inverse_file = None
+    if mask_inverse_img:
+        mask_inverse_file = newfile(roi_output_dir,input_file,prefix="nilearn-mask",suffix=MASK_NAME)
+        nib.save(mask_inverse_img,mask_inverse_file)
+
     NiftiMasker.fit(input_file)
     signals = NiftiMasker.transform(input_file)
     num_rows = signals.shape[0]
 
     # check that rois exist:
     missing_rois = []
     unknown_rois=[]
@@ -317,15 +323,17 @@
     roi_json = os.path.join(roi_output_dir,'{}.json'.format(csv_basename))
     metadata = updateParams(metadata,"Title","roi_extract")
     metadata = updateParams(metadata,"Description","Extract Measures from Image file using provided atlas.")
     metadata = updateParams(metadata,"DateCreated",datetime.datetime.now().strftime("%Y-%m-%d %H:%M:%S:%f"))
     metadata = updateParams(metadata,"Atlas File",atlas_file)
     metadata = updateParams(metadata,"Atlas Labels",atlas_index)
     metadata = updateParams(metadata,"Input File",input_file)
-    metadata = updateParams(metadata,"Command","Nilearn NifiMasker")
+    metadata = updateParams(metadata,"Command","Nilearn NiftiMasker")
+    if mask_inverse_file:
+        metadata = updateParams(metadata,"Mask",mask_inverse_file)
     if metadata_comments:
         metadata = updateParams(metadata,"Comments",metadata_comments)
 
     export_labels(metadata,roi_json)
 
 
     out_files=[]
@@ -341,15 +349,15 @@
 
 
 class roi_extractInputSpec(BaseInterfaceInputSpec):
     labels_dict = traits.Dict({},mandatory=False,desc='labels', usedefault=True)
     input_file = File(desc="input file")
     atlas_file = File(desc='atlas file')
     atlas_index = File(desc='atlas index file')
-    lesion_file = File(desc='lesion file')
+    mask_file = File(desc='mask file')
 
 class roi_extractOutputSpec(TraitedSpec):
     roi_csv = File(desc='CSV file of results')
     roi_output_dir = traits.String(desc='roi output dir')
     output_dir = traits.String(desc='output dir')
     out_files = traits.List(desc='list of files')
     
@@ -361,35 +369,35 @@
 
         # Call our python code here:
         outputs = roi_extract_proc(
             self.inputs.labels_dict,
             self.inputs.input_file,
             self.inputs.atlas_file,
             self.inputs.atlas_index,
-            self.inputs.lesion_file,
+            self.inputs.mask_file,
         )
 
         setattr(self, "_results", outputs)
         # And we are done
         return runtime
 
     def _list_outputs(self):
         return self._results
 
 
-def create(labels_dict,name="roi_extract_node",input_file="",atlas_file="",atlas_index="", lesion_file="", LOGGER=IFLOGGER):
+def create(labels_dict,name="roi_extract_node",input_file="",atlas_file="",atlas_index="", mask_file="", LOGGER=IFLOGGER):
     # Create Node
     pan_node = Node(roi_extract_pan(), name=name)
 
     if LOGGER:
         LOGGER.info(f"Created Node {pan_node!r}")
         
     # Specify node inputs
     pan_node.inputs.labels_dict = labels_dict
     pan_node.inputs.input_file = input_file
     pan_node.inputs.atlas_file =  atlas_file
     pan_node.inputs.atlas_index =  atlas_index
-    pan_node.inputs.lesion_file =  lesion_file
+    pan_node.inputs.mask_file =  mask_file
 
     return pan_node
```

### Comparing `panpipelines-0.9.9/src/panpipelines/nodes/roi_mean_group.py` & `panpipelines-1.0.0/src/panpipelines/nodes/roi_mean_group.py`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.9/src/panpipelines/nodes/roi_mean_single.py` & `panpipelines-1.0.0/src/panpipelines/nodes/roi_mean_single.py`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.9/src/panpipelines/nodes/tensor.py` & `panpipelines-1.0.0/src/panpipelines/nodes/tensor.py`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.9/src/panpipelines/pipelines/aslprep_panpipeline.py` & `panpipelines-1.0.0/src/panpipelines/pipelines/aslprep_panpipeline.py`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.9/src/panpipelines/pipelines/basil_panpipeline.py` & `panpipelines-1.0.0/src/panpipelines/pipelines/basil_panpipeline.py`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.9/src/panpipelines/pipelines/collatecsv_panpipeline.py` & `panpipelines-1.0.0/src/panpipelines/pipelines/collatecsv_panpipeline.py`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.9/src/panpipelines/pipelines/collatecsvgroup_panpipeline.py` & `panpipelines-1.0.0/src/panpipelines/pipelines/collatecsvgroup_panpipeline.py`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.9/src/panpipelines/pipelines/dummy_panpipeline.py` & `panpipelines-1.0.0/src/panpipelines/pipelines/dummy_panpipeline.py`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.9/src/panpipelines/pipelines/fmriprep_panpipeline.py` & `panpipelines-1.0.0/src/panpipelines/pipelines/fmriprep_panpipeline.py`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.9/src/panpipelines/pipelines/freesurfer_panpipeline.py` & `panpipelines-1.0.0/src/panpipelines/pipelines/freesurfer_panpipeline.py`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.9/src/panpipelines/pipelines/lst_panpipeline.py` & `panpipelines-1.0.0/src/panpipelines/pipelines/lst_panpipeline.py`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.9/src/panpipelines/pipelines/noddi_panpipeline.py` & `panpipelines-1.0.0/src/panpipelines/pipelines/noddi_panpipeline.py`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.9/src/panpipelines/pipelines/panpipeline.py` & `panpipelines-1.0.0/src/panpipelines/pipelines/panpipeline.py`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.9/src/panpipelines/pipelines/preproc_panpipeline.py` & `panpipelines-1.0.0/src/panpipelines/pipelines/preproc_panpipeline.py`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.9/src/panpipelines/pipelines/qsiprep_panpipeline.py` & `panpipelines-1.0.0/src/panpipelines/pipelines/qsiprep_panpipeline.py`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.9/src/panpipelines/pipelines/roiextract_panpipeline.py` & `panpipelines-1.0.0/src/panpipelines/pipelines/roiextract_panpipeline.py`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.9/src/panpipelines/pipelines/tensor_panpipeline.py` & `panpipelines-1.0.0/src/panpipelines/pipelines/tensor_panpipeline.py`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.9/src/panpipelines/pipelines/textmeasures_panpipeline.py` & `panpipelines-1.0.0/src/panpipelines/pipelines/textmeasures_panpipeline.py`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.9/src/panpipelines/pipelines/volmeasures_panpipeline.py` & `panpipelines-1.0.0/src/panpipelines/pipelines/volmeasures_panpipeline.py`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.9/src/panpipelines/scripts/aslprep_panscript.py` & `panpipelines-1.0.0/src/panpipelines/scripts/aslprep_panscript.py`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.9/src/panpipelines/scripts/fmriprep_panscript.py` & `panpipelines-1.0.0/src/panpipelines/scripts/fmriprep_panscript.py`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.9/src/panpipelines/scripts/mne_make_surfaces.py` & `panpipelines-1.0.0/src/panpipelines/scripts/mne_make_surfaces.py`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.9/src/panpipelines/scripts/pancontainer_panscript.py` & `panpipelines-1.0.0/src/panpipelines/scripts/pancontainer_panscript.py`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.9/src/panpipelines/scripts/panscript.py` & `panpipelines-1.0.0/src/panpipelines/scripts/panscript.py`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.9/src/panpipelines/scripts/sdcflows_fieldmap.py` & `panpipelines-1.0.0/src/panpipelines/scripts/sdcflows_fieldmap.py`

 * *Files 5% similar despite different names*

```diff
@@ -29,14 +29,15 @@
 
     fm_wf = Workflow(name = "sdcflows_pepolar_wf", base_dir=workdir)
     sinker = Node(DataSink(),name='fmap_sink')
     sinker.inputs.base_directory = os.path.dirname(fieldmap_dir)
     sinker.inputs.substitutions = [
         ('reoriented',f"sub-{subject}_ses-{session}_desc-preproc_fieldmap"),
         ('dir-AP_epi_average_merged_padded_sliced_volreg_base_fieldcoef_fixed',f"desc-coeff_fieldmap"),
+        ('dir-PA_epi_average_merged_padded_sliced_volreg_base_fieldcoef_fixed',f"desc-coeff_fieldmap"),
         ('clipped',f"sub-{subject}_ses-{session}_desc-magnitude_fieldmap")
     ]
     basename = os.path.basename(fieldmap_dir)
     fm_wf.connect( pepolar_wf,"outputnode.fmap",sinker,f"{basename}")
     fm_wf.connect( pepolar_wf,"outputnode.fmap_coeff",sinker,f"{basename}.@coeff")
     fm_wf.connect( pepolar_wf,"outputnode.fmap_mask",sinker,f"{basename}.@mask")
     fm_wf.connect( pepolar_wf,"outputnode.fmap_ref",sinker,f"{basename}.@ref")
```

### Comparing `panpipelines-0.9.9/src/panpipelines/utils/transformer.py` & `panpipelines-1.0.0/src/panpipelines/utils/transformer.py`

 * *Files 1% similar despite different names*

```diff
@@ -94,31 +94,32 @@
 
     from templateflow import api as tf
     mninlin6_mni2009_trans=tf.get("MNI152NLin2009cAsym",suffix="xfm",extension=[".h5"])
     mni2009_t1_ref=tf.get("MNI152NLin2009cAsym",resolution=resolution,desc=None,suffix="T1w",extension=[".nii.gz"])
 
     apply_transform_ants(input_file, mni2009_t1_ref,out_file,mninlin6_mni2009_trans,COMMANDBASE,reverse=reverse, costfunction=costfunction,output_type=output_type)
 
-def apply_transform_ants_ori(input_file,ref_file, out_file, trans_mat, COMMANDBASE, transform_ori="RAS:RAS",target_ori="RAS", reverse=False, costfunction=None, output_type=None):
+
+def apply_transform_ants_ori(input_file,ref_file, out_file, trans_mat, COMMANDBASE, transform_ori=":",target_ori="", reverse=False, costfunction=None, output_type=None):
 
     input_file = os.path.abspath(input_file)
     ref_file=os.path.abspath(ref_file)
     out_file=os.path.abspath(out_file)
 
     expected_mov_ori = transform_ori.split(":")[0]
     expected_ref_ori = transform_ori.split(":")[1]
     
     # Ensure input_file, reference_file and transform are in the same orientation
     ref_ori = get_orientation_from_file(ref_file,"image")
-    if not ref_ori[0] == expected_ref_ori:
+    if expected_ref_ori and ref_ori[0] and not ref_ori[0] == expected_ref_ori:
         print("reorienting  ref_file {} from ref_ori {} to expected_ref_ori {}".format(ref_file, ref_ori, expected_ref_ori))
         ref_file=reorient(ref_file, expected_ref_ori, os.path.dirname(out_file))
 
     mov_ori = get_orientation_from_file(input_file,"image")
-    if not mov_ori[0] == expected_mov_ori:
+    if expected_mov_ori  and mov_ori[0] and not mov_ori[0] == expected_mov_ori:
         print("reorienting input_file (moving) {} from mov_ori {} to expected_mov_ori {}".format(input_file, mov_ori, expected_mov_ori))
         input_file=reorient(input_file, expected_mov_ori, os.path.dirname(out_file))
 
     if costfunction is None:
         costfunction="LanczosWindowedSinc"
 
     img = nib.load(input_file)
@@ -176,15 +177,15 @@
     command=f"{COMMANDBASE} fslroi"\
             " "+out_file+" "+out_file + " 0 "+str(dimz)
     results = ut.runCommand(command)
 
     # Transform to target orientation
     # Ensure input_file, reference_file and transform are in the same orientation
     actual_target_ori = get_orientation_from_file(out_file,"image")
-    if not actual_target_ori[0] == target_ori:
+    if target_ori and not actual_target_ori[0] == target_ori:
         print("reorienting  target_file {} from actual_target_ori {} to {}".format(out_file, actual_target_ori, target_ori))
         out_file=reorient(out_file, target_ori,out_file)
 
     return out_file
 
 
 def apply_transform_ants(input_file,ref_file, out_file, trans_mat, COMMANDBASE, reverse=False, costfunction=None,output_type=None):
@@ -809,15 +810,15 @@
     
     fnirt_inv_field = tempfile.mkstemp()[1] + ".nii.gz"
     invertWarpfield_FNIRT(orig_source, fnirt_fwd_field, fnirt_inv_field , COMMANDBASE)
     
     convertwarp_toANTS(fnirt_inv_field,orig_destination, ants_inv_field, COMMANDBASE,absolute)
 
 def invertAffine_FLIRT(fwd_affine, inv_affine, COMMANDBASE):
-    command=f"{COMMANDBASE} comvert_xfm"\
+    command=f"{COMMANDBASE} convert_xfm"\
         f" -omat {inv_affine}"\
         f" -inverse"\
         f" {fwd_affine}"
     results = ut.runCommand(command)
 
 def invertAffine_ANTS(fwd_affine, inv_affine, moving, reference, COMMANDBASE):
     fsl_fwd_affine = tempfile.mkstemp()[1] + ".mat"
```

### Comparing `panpipelines-0.9.9/src/panpipelines/utils/util_functions.py` & `panpipelines-1.0.0/src/panpipelines/utils/util_functions.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 import shutil
 from panpipelines.utils.transformer import *
 import sys
 from nipype import logging as nlogging
 import fcntl
 import time
 from bids import BIDSLayout
+from collections import OrderedDict
 
 UTLOGGER=nlogging.getLogger('nipype.utils')
 
 def logger_setup(logname, loglevel):
     LOGGER = logging.getLogger(logname)
     LOGGER.setLevel(loglevel)
     return LOGGER
@@ -981,14 +982,88 @@
         pass
     except TypeError as te:
         pass
     
     return int(np.min(np.array(procnum_list)))
 
 
+def add_mask_roi(atlas_file, roi_in, panpipe_labels, high_thresh=None,prob_thresh=0.5,roi_transform=None,invert_roi=False):
+
+    workdir = os.path.join(os.path.dirname(atlas_file),'roi_temp')
+    if not os.path.isdir(workdir):
+        os.makedirs(workdir)
+
+    trans_workdir = os.path.join(os.path.dirname(atlas_file),'roi_transformed')
+    if not os.path.isdir(trans_workdir):
+        os.makedirs(trans_workdir)
+
+    if prob_thresh:
+        PROBTHRESH=f" -thr {prob_thresh}"
+    else:
+        PROBTHRESH=""
+
+    if high_thresh:
+        HIGHTHRESH=f" -uthr {high_thresh}"
+    else:
+        HIGHTHRESH = ""
+
+    if invert_roi:
+        BINSTRING = " -binv"
+    else:
+        BINSTRING = " -bin"
+
+
+    # store roi in work dir for
+    command_base, container = getContainer(panpipe_labels,nodename="add_atlas_roi",SPECIFIC="NEURO_CONTAINER")
+    new_roi=newfile(trans_workdir, roi_in, suffix="desc-label")
+    command = f"{command_base} fslmaths"\
+        f"  {roi_in}" +\
+        HIGHTHRESH +\
+        PROBTHRESH +\
+        BINSTRING +\
+        f" {new_roi}" 
+    
+    evaluated_command=substitute_labels(command,panpipe_labels)
+    results = runCommand(evaluated_command)
+
+    from panpipelines.nodes.antstransform import antstransform_proc
+
+    roi_transform_ref = getParams(panpipe_labels,"ROI_TRANSFORM_REF")
+    if roi_transform:
+        CURRDIR = os.getcwd()
+        os.chdir(trans_workdir)
+        results = antstransform_proc(panpipe_labels, new_roi,roi_transform, roi_transform_ref)
+        new_roi_transformed = results['out_file']
+        os.chdir(CURRDIR)
+    else:
+        new_roi_transformed = newfile(trans_workdir, new_roi)
+        shutil.move(new_roi, new_roi_transformed)
+
+    # make output file into int. This was initially don in ANTS above but had issues with rois that had value of 1
+    command = f"{command_base} fslmaths"\
+            f"  {new_roi_transformed}"\
+            f" {new_roi_transformed}" \
+             " -odt int"
+    evaluated_command=substitute_labels(command,panpipe_labels)
+    results = runCommand(evaluated_command)
+
+    if os.path.exists(atlas_file):
+        command = f"{command_base} fslmaths"\
+            f"  {new_roi_transformed}"\
+            f" -mas {atlas_file}" +\
+            f" {atlas_file}"
+    else:
+        command = f"{command_base} fslmaths"\
+            f" {new_roi_transformed}"\
+            f" {atlas_file}" 
+    
+    evaluated_command=substitute_labels(command,panpipe_labels)
+    results = runCommand(evaluated_command)
+
+
 def add_atlas_roi(atlas_file, roi_in, roi_value, panpipe_labels, high_thresh=None,low_thresh=None,prob_thresh=0.5,roi_transform=None):
 
     workdir = os.path.join(os.path.dirname(atlas_file),'roi_temp')
     if not os.path.isdir(workdir):
         os.makedirs(workdir)
 
     trans_workdir = os.path.join(os.path.dirname(atlas_file),'roi_transformed')
@@ -1073,15 +1148,62 @@
     # create rois
     for roi_num in range(numrois):
         roi = roi_list[roi_num]
         roi_transform=None
         if roi_transform_mat and roi_num < len(roi_transform_mat):
             roi_transform = roi_transform_mat[roi_num]
         roi_value = roi_values[roi_num]
-        add_atlas_roi(atlas_file, roi, roi_value, panpipe_labels,high_thresh=roi_value,prob_thresh=prob_thresh,roi_transform=roi_transform)
+        if isinstance(prob_thresh,list):
+            prob_thresh_val = float(prob_thresh[np.min((roi_num,len(prob_thresh)-1))])
+        elif prob_thresh:
+            prob_thresh_val = prob_thresh
+        else:
+            prob_thresh_val = ""
+
+        add_atlas_roi(atlas_file, roi, roi_value, panpipe_labels,high_thresh=roi_value,prob_thresh=prob_thresh_val,roi_transform=roi_transform)
+
+    return atlas_file
+
+def create_3d_mask_from_rois(atlas_file, roi_list,panpipe_labels, roi_values=None,prob_thresh=0.5,explode3d=True,invert_roi=False):
+
+    roi_list = expand_rois(roi_list,os.path.dirname(atlas_file),panpipe_labels,explode3d=explode3d)
+    roi_transform_mat = getParams(panpipe_labels,"ROI_TRANSFORM_MAT")
+    panpipe_labels=updateParams(panpipe_labels,"ROI_TRANSFORM_REF",getParams(panpipe_labels,"NEWATLAS_TRANSFORM_REF"))
+
+    numrois=len(roi_list)
+
+    # create rois
+    for roi_num in range(numrois):
+        roi = roi_list[roi_num]
+        roi_transform=None
+        if roi_transform_mat and roi_num < len(roi_transform_mat):
+            roi_transform = roi_transform_mat[roi_num]
+
+        if isinstance(roi_values,list):
+            roi_value = float(roi_values[np.min((roi_num,len(roi_values)-1))])
+        elif prob_thresh:
+            roi_value = roi_values
+        else:
+            roi_value = None
+
+        if isinstance(prob_thresh,list):
+            prob_thresh_val = float(prob_thresh[np.min((roi_num,len(prob_thresh)-1))])
+        elif prob_thresh:
+            prob_thresh_val = prob_thresh
+        else:
+            prob_thresh_val = 0.5
+
+        if isinstance(invert_roi,list):
+            invert_roi_val = isTrue(invert_roi[np.min((roi_num,len(invert_roi)-1))])
+        elif invert_roi:
+            invert_roi_val = invert_roi
+        else:
+            invert_roi_val = False
+
+        add_mask_roi(atlas_file, roi, panpipe_labels,high_thresh=roi_value,prob_thresh=prob_thresh_val,roi_transform=roi_transform,invert_roi=invert_roi_val)
 
     return atlas_file
 
 def merge_atlas_roi(atlas_file, roi_list, panpipe_labels, high_thresh=None,low_thresh=None):
 
     workdir = os.path.join(os.path.dirname(atlas_file),'roi_temp')
     if not os.path.isdir(workdir):
@@ -1092,37 +1214,44 @@
         os.makedirs(trans_workdir)
 
     if high_thresh:
         HIGHTHRESH=f" -uthr {high_thresh}"
     else:
         HIGHTHRESH = ""
 
-    if low_thresh:
-        LOWTHRESH=f" -thr {low_thresh}"
-    else:
-        LOWTHRESH=""
-
     command_base, container = getContainer(panpipe_labels,nodename="merge_atlas_roi",SPECIFIC="NEURO_CONTAINER")
 
     roicount=0
     numrois=len(roi_list)
     roi_files=[]
     for roi_in in roi_list:       
         # store roi in work dir\
-        roicount=roicount+1
+        if isinstance(low_thresh,list):
+            low_thresh_val = float(low_thresh[np.min((roicount,len(low_thresh)-1))])
+        elif low_thresh:
+            low_thresh_val = low_thresh
+        else:
+            low_thresh_val = ""
+
+        if low_thresh_val:
+            LOWTHRESH=f" -thr {low_thresh_val}"
+        else:
+            LOWTHRESH=""
+        
         new_roi=newfile(workdir, roi_in,suffix="desc-bin")
         command = f"{command_base} fslmaths"\
             f"  {roi_in}" +\
             LOWTHRESH +\
             HIGHTHRESH +\
             " -bin "\
             f" {new_roi}"
         evaluated_command=substitute_labels(command,panpipe_labels)
         results = runCommand(evaluated_command)
         roi_files.append(new_roi)
+        roicount=roicount+1
 
     from panpipelines.nodes.antstransform import antstransform_proc
     roi_files_transformed=[]
     roi_transform_mat = getParams(panpipe_labels,"ROI_TRANSFORM_MAT")
     roi_transform_ref = getParams(panpipe_labels,"ROI_TRANSFORM_REF")
     for roi_num in range(len(roi_files)):
         if roi_transform_mat and roi_num < len(roi_transform_mat):
@@ -1872,8 +2001,156 @@
     return bidslist
 
 
 def getPepolarSources(bids_dir,participant_label,participant_session=None,acquisition="fmri",datatype="fmap",suffix=['epi'],extension="nii.gz"):   
     layout = BIDSLayout(bids_dir)
     bidslist = layout.get(return_type='file',subject=participant_label,session=participant_session,acquisition=acquisition,datatype=datatype,suffix=suffix,extension=extension)
 
-    return bidslist
+    return bidslist
+
+
+def get_fslparams(fsl_dict):
+    params = ""
+    for fsl_tag, fsl_value in fsl_dict.items():
+        if "--" in fsl_tag and "---" not in fsl_tag:
+            if fsl_value == "^^^":
+                    params=params + " " + fsl_tag
+            elif fsl_value == "###":
+                UTLOGGER.info(f"Parameter {fsl_tag} is being skipped. This has been explicitly required in configuration.")
+            else:
+                if fsl_value:
+                    params = params + " " + fsl_tag+"=" + str(fsl_value)
+
+        elif str(fsl_tag).upper().startswith("DUMMYKEY") and fsl_value:
+                params=params + " " + fsl_value
+        elif "-" in fsl_tag and "--" not in fsl_tag:
+            if fsl_value == "^^^":
+                    params=params + " " + fsl_tag
+            elif fsl_value == "###":
+                UTLOGGER.info(f"Parameter {fsl_tag} is being skipped. This has been explicitly required in configuration.")
+            else:
+                if fsl_value:
+                    params = params + " " + fsl_tag +" " + str(fsl_value)
+
+        else:
+            print(f"fsl tag {fsl_tag} not valid.")
+    return params
+
+def N4BiasFieldCorrection(panpipe_labels,inputfile,biascorr_output,biascorr_field=None,mask=None,dims=3,spline_spacing="[ 180 ]",convergence="[ 50x50x50x50, 0.0]",shrink_factor="1"):
+    command_base, container = getContainer(panpipe_labels,nodename="N4BiasFieldCorrection",SPECIFIC="ANTS_CONTAINER",LOGGER=UTLOGGER)
+
+    if not biascorr_field:
+        biascorr_field = newfile(assocfile=biascorr_output,suffix="biascorr-field")
+
+    ants_dict=OrderedDict()
+    ants_dict = updateParams(ants_dict,"-d",str(dims))
+    ants_dict = updateParams(ants_dict,"-v","1")
+    ants_dict = updateParams(ants_dict,"-s",str(shrink_factor))
+    ants_dict = updateParams(ants_dict,"-b",str(spline_spacing))
+    ants_dict = updateParams(ants_dict,"-c",str(convergence))
+    ants_dict = updateParams(ants_dict,"-i",str(inputfile))
+    ants_dict = updateParams(ants_dict,"-o",f"[ {str(biascorr_output)},{biascorr_field} ]")
+    ants_dict = updateParams(ants_dict,"-m",mask)
+
+    params = get_fslparams(ants_dict)
+    command=f"{command_base} N4BiasFieldCorrection"\
+        " "+params
+    evaluated_command=substitute_labels(command, panpipe_labels)
+    results = runCommand(evaluated_command,UTLOGGER)
+
+
+def clean_up_edge(panpipe_labels, outfile, maskim, tmpnm, despike_thresh=2.1,edge_thresh=0.5):
+    command_base, container = getContainer(panpipe_labels,nodename="clean_up_edge",SPECIFIC="FSL_CONTAINER",LOGGER=UTLOGGER)
+
+    fsl_dict=OrderedDict()
+    fsl_dict = updateParams(fsl_dict,"--loadfmap",f"{str(outfile)}")
+    fsl_dict = updateParams(fsl_dict,"--savefmap",f"{str(tmpnm)}_tmp_fmapfilt")
+    fsl_dict = updateParams(fsl_dict,"--mask",f"{str(maskim)}")
+    fsl_dict = updateParams(fsl_dict,"--despike","^^^")
+    fsl_dict = updateParams(fsl_dict,"--despikethreshold",f"{str(despike_thresh)}")
+    params = get_fslparams(fsl_dict)
+    command=f"{command_base} fugue"\
+        " "+params
+    evaluated_command=substitute_labels(command, panpipe_labels)
+    results = runCommand(evaluated_command,UTLOGGER)
+
+    fsl_dict=OrderedDict()
+    fsl_dict = updateParams(fsl_dict,"DUMMYKEY0",f"{str(maskim)}")
+    fsl_dict = updateParams(fsl_dict,"-kernel","2D")
+    fsl_dict = updateParams(fsl_dict,"-ero",f"{str(tmpnm)}_tmp_eromask")
+
+    params = get_fslparams(fsl_dict)
+    command=f"{command_base} fslmaths"\
+        " "+params
+    evaluated_command=substitute_labels(command, panpipe_labels)
+    results = runCommand(evaluated_command,UTLOGGER)
+
+    fsl_dict=OrderedDict()
+    fsl_dict = updateParams(fsl_dict,"DUMMYKEY0",f"{str(maskim)}")
+    fsl_dict = updateParams(fsl_dict,"-sub",f"{str(tmpnm)}_tmp_eromask")
+    fsl_dict = updateParams(fsl_dict,"-thr",f"{str(edge_thresh)}")
+    fsl_dict = updateParams(fsl_dict,"-bin",f"{str(tmpnm)}_tmp_edgemask")
+
+    params = get_fslparams(fsl_dict)
+    command=f"{command_base} fslmaths"\
+        " "+params
+    evaluated_command=substitute_labels(command, panpipe_labels)
+    results = runCommand(evaluated_command,UTLOGGER)
+
+    fsl_dict=OrderedDict()
+    fsl_dict = updateParams(fsl_dict,"DUMMYKEY0",f"{str(tmpnm)}_tmp_fmapfilt")
+    fsl_dict = updateParams(fsl_dict,"-mas",f"{str(tmpnm)}_tmp_edgemask")
+    fsl_dict = updateParams(fsl_dict,"DUMMYKEY1",f"{str(tmpnm)}_tmp_fmapfiltedge")
+
+    params = get_fslparams(fsl_dict)
+    command=f"{command_base} fslmaths"\
+        " "+params
+    evaluated_command=substitute_labels(command, panpipe_labels)
+    results = runCommand(evaluated_command,UTLOGGER)
+
+    fsl_dict=OrderedDict()
+    fsl_dict = updateParams(fsl_dict,"DUMMYKEY0",f"{str(outfile)}")
+    fsl_dict = updateParams(fsl_dict,"-mas",f"{str(tmpnm)}_tmp_eromask")
+    fsl_dict = updateParams(fsl_dict,"-add",f"{str(tmpnm)}_tmp_fmapfiltedge")
+    fsl_dict = updateParams(fsl_dict,"DUMMYKEY1",f"{str(outfile)}")
+
+    params = get_fslparams(fsl_dict)
+    command=f"{command_base} fslmaths"\
+        " "+params
+    evaluated_command=substitute_labels(command, panpipe_labels)
+    results = runCommand(evaluated_command,UTLOGGER)
+
+
+def demean_image(panpipe_labels, outim, maskim, tmpnm, percentile=50):
+    command_base, container = getContainer(panpipe_labels,nodename="demean_image",SPECIFIC="FSL_CONTAINER",LOGGER=UTLOGGER)
+
+    fsl_dict=OrderedDict()
+    fsl_dict = updateParams(fsl_dict,"DUMMYKEY0",f"{str(outim)}")
+    fsl_dict = updateParams(fsl_dict,"-mas",f"{maskim}")
+    fsl_dict = updateParams(fsl_dict,"DUMMYKEY1",f"{str(tmpnm)}_tmp_fmapmasked")
+    params = get_fslparams(fsl_dict)
+    command=f"{command_base} fslmaths"\
+        " "+params
+    evaluated_command=substitute_labels(command, panpipe_labels)
+    results = runCommand(evaluated_command,UTLOGGER)
+
+    fsl_dict=OrderedDict()
+    fsl_dict = updateParams(fsl_dict,"DUMMYKEY0",f"{str(tmpnm)}_tmp_fmapmasked")
+    fsl_dict = updateParams(fsl_dict,"-k",f"{maskim}")
+    fsl_dict = updateParams(fsl_dict,"-P",f"{str(percentile)}")
+    params = get_fslparams(fsl_dict)
+    command=f"{command_base} fslstats"\
+        " "+params
+    evaluated_command=substitute_labels(command, panpipe_labels)
+    subfactor = runCommand(evaluated_command,UTLOGGER).strip()
+
+    fsl_dict=OrderedDict()
+    fsl_dict = updateParams(fsl_dict,"DUMMYKEY0",f"{str(outim)}")
+    fsl_dict = updateParams(fsl_dict,"-sub",f"{subfactor}")
+    fsl_dict = updateParams(fsl_dict,"-mas",f"{maskim}")
+    fsl_dict = updateParams(fsl_dict,"DUMMYKEY1",f"{str(outim)}")
+    fsl_dict = updateParams(fsl_dict,"-odt","float")
+    params = get_fslparams(fsl_dict)
+    command=f"{command_base} fslmaths"\
+        " "+params
+    evaluated_command=substitute_labels(command, panpipe_labels)
+    results = runCommand(evaluated_command,UTLOGGER)
```

### Comparing `panpipelines-0.9.9/src/panpipelines/workflows/aslprep_workflow.py` & `panpipelines-1.0.0/src/panpipelines/workflows/aslprep_workflow.py`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.9/src/panpipelines/workflows/basil_workflow.py` & `panpipelines-1.0.0/src/panpipelines/workflows/basil_workflow.py`

 * *Files 20% similar despite different names*

```diff
@@ -16,32 +16,56 @@
 
     if LOGGER:
         LOGGER.info(f"Created Workflow {name} with base directory {wf_base_dir}")
 
     if len(execution.keys()) > 0:
         pan_workflow.config = process_dict(pan_workflow.config,execution)
 
-    # Specify node inputs
-    fslanat_manual=getParams(labels_dict,"FSLANAT_MANUAL")
-    if fslanat_manual and fslanat_manual == "Y":
-        fslanat_dir=getParams(labels_dict,"FSLANAT_DIR")
-        basil_node = basil.create(labels_dict,fslanat_dir=fslanat_dir,LOGGER=LOGGER)
-        pan_workflow.add_nodes([basil_node])
-    else:
-        fslanat_node = fslanat.create(labels_dict,LOGGER=LOGGER)
-        basil_node = basil.create(labels_dict,LOGGER=LOGGER)
-        pan_workflow.connect(fslanat_node,'fslanat_dir',basil_node,'fslanat_dir')
-
+    bids_dir = getParams(labels_dict,"BIDS_DIR")
+    participant_label = getParams(labels_dict,'PARTICIPANT_LABEL')
+    participant_session = getParams(labels_dict,'PARTICIPANT_SESSION')
+    acq_label = getAcquisition(bids_dir,participant_label,participant_session=participant_session)
+
+    use_pepolar_fmap = getParams(labels_dict,'USE_PEPOLAR_FMAP')
+    if use_pepolar_fmap and participant_label in use_pepolar_fmap:
+        sdcflows_fmap_mode="pepolar"
+        labels_dict = updateParams(labels_dict,"SDCFLOWS_FIELDMAP_MODE",sdcflows_fmap_mode)
+        labels_dict = updateParams(labels_dict,"FIELDMAP_TYPE","sdcflows_preproc")
+        if not getParams(labels_dict,"SDCFLOWS_FIELDMAP_DIR"):
+            labels_dict = updateParams(labels_dict,"SDCFLOWS_FIELDMAP_DIR","<WORKFLOW_DIR>/sdcflows/fmap")
+    elif use_pepolar_fmap and f"{participant_label}_{participant_session}" in use_pepolar_fmap:
+        sdcflows_fmap_mode="pepolar"
+        labels_dict = updateParams(labels_dict,"SDCFLOWS_FIELDMAP_MODE",sdcflows_fmap_mode)
+        labels_dict = updateParams(labels_dict,"FIELDMAP_TYPE","sdcflows_preproc")
+        if not getParams(labels_dict,"SDCFLOWS_FIELDMAP_DIR"):
+            labels_dict = updateParams(labels_dict,"SDCFLOWS_FIELDMAP_DIR","<WORKFLOW_DIR>/sdcflows/fmap")
+
+    use_phasediff_fmap = getParams(labels_dict,'USE_PHASEDIFF_FMAP')
+    if use_phasediff_fmap and participant_label in use_phasediff_fmap:
+        sdcflows_fmap_mode="phasediff"
+        labels_dict = updateParams(labels_dict,"SDCFLOWS_FIELDMAP_MODE",sdcflows_fmap_mode)
+        labels_dict = updateParams(labels_dict,"FIELDMAP_TYPE","sdcflows_preproc")
+        if not getParams(labels_dict,"SDCFLOWS_FIELDMAP_DIR"):
+            labels_dict = updateParams(labels_dict,"SDCFLOWS_FIELDMAP_DIR","<WORKFLOW_DIR>/sdcflows/fmap")
+    elif use_phasediff_fmap and f"{participant_label}_{participant_session}" in use_phasediff_fmap:
+        sdcflows_fmap_mode="phasediff"
+        labels_dict = updateParams(labels_dict,"SDCFLOWS_FIELDMAP_MODE",sdcflows_fmap_mode)
+        labels_dict = updateParams(labels_dict,"FIELDMAP_TYPE","sdcflows_preproc")
+        if not getParams(labels_dict,"SDCFLOWS_FIELDMAP_DIR"):
+            labels_dict = updateParams(labels_dict,"SDCFLOWS_FIELDMAP_DIR","<WORKFLOW_DIR>/sdcflows/fmap")
+
+    use_phasediff_manual_fmap = getParams(labels_dict,'USE_PHASEDIFF_MANUAL_FMAP')
+    if use_phasediff_manual_fmap and participant_label in use_phasediff_manual_fmap:
+        labels_dict = updateParams(labels_dict,"FIELDMAP_TYPE","fsl_prepare_fieldmap")
+    elif use_phasediff_manual_fmap and f"{participant_label}_{participant_session}" in use_phasediff_manual_fmap:
+        labels_dict = updateParams(labels_dict,"FIELDMAP_TYPE","fsl_prepare_fieldmap")
+    
     FIELDMAP_TYPE = getParams(labels_dict,"FIELDMAP_TYPE")
     SDCFLOWS_FMAP_DIR = getParams(labels_dict,"SDCFLOWS_FIELDMAP_DIR")
     if FIELDMAP_TYPE and SDCFLOWS_FMAP_DIR:
-        bids_dir = getParams(labels_dict,"BIDS_DIR")
-        participant_label = getParams(labels_dict,'PARTICIPANT_LABEL')
-        participant_session = getParams(labels_dict,'PARTICIPANT_SESSION')
-        acq_label = getAcquisition(bids_dir,participant_label,participant_session=participant_session)
         if isinstance(FIELDMAP_TYPE,dict):
             if acq_label in FIELDMAP_TYPE.keys():
                 FIELDMAP_TYPE = FIELDMAP_TYPE[acq_label]   
 
         if FIELDMAP_TYPE == "sdcflows_preproc":
             if isinstance(SDCFLOWS_FMAP_DIR,dict):
                 if acq_label in SDCFLOWS_FMAP_DIR.keys():
@@ -55,27 +79,14 @@
             SDCFLOWS_FMAP_DIR=substitute_labels(SDCFLOWS_FMAP_DIR,labels_dict)
     
             SDCFLOWS_FMAP_MODE = getParams(labels_dict,"SDCFLOWS_FIELDMAP_MODE") 
             if SDCFLOWS_FMAP_MODE:
                 sdcflows_fmap_mode = SDCFLOWS_FMAP_MODE
             else:
                 sdcflows_fmap_mode="phasediff"          
-
-            use_pepolar_fmap = getParams(labels_dict,'USE_PEPOLAR_FMAP')
-            if use_pepolar_fmap and participant_label in use_pepolar_fmap:
-                sdcflows_fmap_mode="pepolar"
-            elif use_pepolar_fmap and f"{participant_label}_{participant_session}" in use_pepolar_fmap:
-                sdcflows_fmap_mode="pepolar"
-
-            use_phasediff_fmap = getParams(labels_dict,'USE_PHASEDIFF_FMAP')
-            if use_phasediff_fmap and participant_label in use_phasediff_fmap:
-                sdcflows_fmap_mode="phasediff"
-            elif use_phasediff_fmap and f"{participant_label}_{participant_session}" in use_phasediff_fmap:
-                sdcflows_fmap_mode="phasediff"
-            labels_dict = updateParams(labels_dict,"SDCFLOWS_FIELDMAP_MODE",sdcflows_fmap_mode)
             
             sdcflows_workdir = os.path.dirname(SDCFLOWS_FMAP_DIR)
             if not os.path.exists(sdcflows_workdir):
                 os.makedirs(sdcflows_workdir)
 
             sdcflows_fmap_parentdir = os.path.dirname(SDCFLOWS_FMAP_DIR)
             if not os.path.exists(sdcflows_fmap_parentdir):
@@ -110,12 +121,23 @@
                     panscript = pancontainer_script.pancontainer_panscript(labels_dict,params=params,command=f"python {sdcflows_fieldmap.__file__}")
                 panscript.run()
             else:
                 if LOGGER:
                     LOGGER.warn("Attempting to create fieldmap but sources not found. Exiting")
                 sys.exit(1)
 
+        # Specify node inputs
+    fslanat_manual=getParams(labels_dict,"FSLANAT_MANUAL")
+    if fslanat_manual and fslanat_manual == "Y":
+        fslanat_dir=getParams(labels_dict,"FSLANAT_DIR")
+        basil_node = basil.create(labels_dict,fslanat_dir=fslanat_dir,LOGGER=LOGGER)
+        pan_workflow.add_nodes([basil_node])
+    else:
+        fslanat_node = fslanat.create(labels_dict,LOGGER=LOGGER)
+        basil_node = basil.create(labels_dict,LOGGER=LOGGER)
+        pan_workflow.connect(fslanat_node,'fslanat_dir',basil_node,'fslanat_dir')
+
             
     if createGraph:
          pan_workflow.write_graph(graph2use='flat')
 
     return pan_workflow
```

### Comparing `panpipelines-0.9.9/src/panpipelines/workflows/collatecsv_workflow.py` & `panpipelines-1.0.0/src/panpipelines/workflows/collatecsv_workflow.py`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.9/src/panpipelines/workflows/collatecsvgroup_workflow.py` & `panpipelines-1.0.0/src/panpipelines/workflows/collatecsvgroup_workflow.py`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.9/src/panpipelines/workflows/dummy_workflow.py` & `panpipelines-1.0.0/src/panpipelines/workflows/dummy_workflow.py`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.9/src/panpipelines/workflows/fmriprep_workflow.py` & `panpipelines-1.0.0/src/panpipelines/workflows/fmriprep_workflow.py`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.9/src/panpipelines/workflows/freesurfer_workflow.py` & `panpipelines-1.0.0/src/panpipelines/workflows/freesurfer_workflow.py`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.9/src/panpipelines/workflows/lst_workflow.py` & `panpipelines-1.0.0/src/panpipelines/workflows/lst_workflow.py`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.9/src/panpipelines/workflows/noddi_workflow.py` & `panpipelines-1.0.0/src/panpipelines/workflows/noddi_workflow.py`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.9/src/panpipelines/workflows/preproc_workflow.py` & `panpipelines-1.0.0/src/panpipelines/workflows/preproc_workflow.py`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.9/src/panpipelines/workflows/qsiprep_workflow.py` & `panpipelines-1.0.0/src/panpipelines/workflows/qsiprep_workflow.py`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.9/src/panpipelines/workflows/roiextract_workflow.py` & `panpipelines-1.0.0/src/panpipelines/workflows/roiextract_workflow.py`

 * *Files 17% similar despite different names*

```diff
@@ -13,58 +13,81 @@
 
     if LOGGER:
         LOGGER.info(f"Created Workflow {name} with base directory {wf_base_dir}")
 
     if len(execution.keys()) > 0:
         pan_workflow.config = process_dict(pan_workflow.config,execution)
 
-    # do we have  a lesion to exclude?
-    lesioncreate_node = None
-    lesion_templates = getParams(labels_dict,"LESION_TEMPLATE")
-    if lesion_templates:
-        lesion_list=[]
-        lesion_name = getParams(labels_dict,"LESION_NAME")
-        if not lesion_name:
-            lesion_name="lesion"
-        lesion_index = getParams(labels_dict,"LESION_INDEX")
-        if isinstance(lesion_templates,list):
-            for lesion_template in lesion_templates:
-                evaluated_lesion_template = substitute_labels(lesion_template,labels_dict)
-                if "*" not in evaluated_lesion_template:
-                    lesion_list.append(evaluated_lesion_template)
+    # do we have  a mask to exclude?
+    maskcreate_node = None
+    mask_templates = getParams(labels_dict,"MASK_TEMPLATE")
+    if mask_templates:
+        mask_list=[]
+        mask_name = getParams(labels_dict,"MASK_NAME")
+        if not mask_name:
+            mask_name="mask"
+        mask_index = getParams(labels_dict,"MASK_INDEX")
+        if isinstance(mask_templates,list):
+            for mask_template in mask_templates:
+                evaluated_mask_template = substitute_labels(mask_template,labels_dict)
+                if "*" not in evaluated_mask_template:
+                    mask_list.append(evaluated_mask_template)
                 else:
-                    lesion_list.extend(glob.glob(evaluated_lesion_template))
+                    mask_list.extend(glob.glob(evaluated_mask_template))
         else:
-            lesion_list.extend(glob.glob(lesion_templates))
+            mask_list.extend(glob.glob(mask_templates))
 
-        # if lesion template is invalid then continue, otherwise print message and continue without
-        # using lesion segmenntation
-        LESION_TEMPLATE_EXISTS=True
-        for lesion in lesion_list:
-            if not os.path.exists(lesion):
-                LESION_TEMPLATE_EXISTS = False
+        # if mask template is invalid then continue, otherwise print message and continue without
+        # using mask segmenntation
+        MASK_TEMPLATE_EXISTS=True
+        for mask in mask_list:
+            if not os.path.exists(mask):
+                MASK_TEMPLATE_EXISTS = False
 
-        if lesion_list and LESION_TEMPLATE_EXISTS:    
-            # store and restore parameters used by both lesion and newatlas
+        if mask_list and MASK_TEMPLATE_EXISTS and getParams(labels_dict,"MASK_TRANSFORM_MAT"):    
+            # store and restore parameters used by both mask and newatlas
             newatlas_transform_mat = getParams(labels_dict,"NEWATLAS_TRANSFORM_MAT")
             newatlas_transform_ref = getParams(labels_dict,"NEWATLAS_TRANSFORM_REF")
-            lesion_transform_mat = getParams(labels_dict,"LESION_TRANSFORM_MAT")
-            lesion_transform_ref = getParams(labels_dict,"LESION_TRANSFORM_REF")
-
-            labels_dict = updateParams(labels_dict,"NEWATLAS_TRANSFORM_MAT",lesion_transform_mat)
-            labels_dict = updateParams(labels_dict,"NEWATLAS_TRANSFORM_REF",lesion_transform_ref)
+            newatlas_type = getParams(labels_dict,"NEWATLAS_TYPE")
+            newatlas_name = getParams(labels_dict,"NEWATLAS_NAME")
+            newatlas_probthresh = getParams(labels_dict,"NEWATLAS_PROBTHRESH")
+            newatlas_invertroi = getParams(labels_dict,"NEWATLAS_INVERTROI")
+            newatlas_indexmode = getParams(labels_dict,"NEWATLAS_INDEXMODE")
+
+            mask_transform_mat = getParams(labels_dict,"MASK_TRANSFORM_MAT")
+            mask_transform_ref = getParams(labels_dict,"MASK_TRANSFORM_REF")
+            mask_type = getParams(labels_dict,"MASK_TYPE")
+            if not mask_type:
+                mask_type = "3D_mask"
+            mask_name = getParams(labels_dict,"MASK_NAME")
+            mask_probthresh = getParams(labels_dict,"MASK_PROBTHRESH")
+            mask_invertroi = getParams(labels_dict,"MASK_INVERTROI")
+            mask_indexmode = getParams(labels_dict,"MASK_INDEXMODE")
+
+            labels_dict = updateParams(labels_dict,"NEWATLAS_TRANSFORM_MAT",mask_transform_mat)
+            labels_dict = updateParams(labels_dict,"NEWATLAS_TRANSFORM_REF",mask_transform_ref)
+            labels_dict = updateParams(labels_dict,"NEWATLAS_TYPE",mask_type)
+            labels_dict = updateParams(labels_dict,"NEWATLAS_NAME",mask_name)
+            labels_dict = updateParams(labels_dict,"NEWATLAS_PROBTHRESH",mask_probthresh)
+            labels_dict = updateParams(labels_dict,"NEWATLAS_INVERTROI",mask_invertroi)
+            labels_dict = updateParams(labels_dict,"NEWATLAS_INDEXMODE",mask_indexmode)
 
             labels_dict = updateParams(labels_dict,"COST_FUNCTION","NearestNeighbor")
-            lesioncreate_node = atlascreate.create(labels_dict,name=f"lesioncreate_{lesion_name}_node",roi_list=lesion_list,roilabels_list=lesion_index,LOGGER=LOGGER)
+            maskcreate_node = atlascreate.create(labels_dict,name=f"maskcreate_{mask_name}_node",roi_list=mask_list,roilabels_list=mask_index,LOGGER=LOGGER)
 
             labels_dict = updateParams(labels_dict,"NEWATLAS_TRANSFORM_MAT",newatlas_transform_mat)
             labels_dict = updateParams(labels_dict,"NEWATLAS_TRANSFORM_REF",newatlas_transform_ref)
+            labels_dict = updateParams(labels_dict,"NEWATLAS_TYPE",newatlas_type)
+            labels_dict = updateParams(labels_dict,"NEWATLAS_NAME",newatlas_name)
+            labels_dict = updateParams(labels_dict,"NEWATLAS_PROBTHRESH",newatlas_probthresh)
+            labels_dict = updateParams(labels_dict,"NEWATLAS_INVERTROI",newatlas_invertroi)
+            labels_dict = updateParams(labels_dict,"NEWATLAS_INDEXMODE",newatlas_indexmode)
         else:
             if LOGGER:
-                LOGGER.info(f"Lesion Template defined but valid template file not found. Ignoring Lesion Template.")
+                LOGGER.info(f"mask Template defined but valid template file not found. Ignoring mask Template.")
 
     # do we need to create a custom atlas?
     atlas_index = getParams(labels_dict,"ATLAS_INDEX")
     atlas_file = getParams(labels_dict,"ATLAS_FILE")
     atlas_name = getParams(labels_dict,"ATLAS_NAME")
     atlascreate_node=None
     if not atlas_file:
@@ -135,16 +158,19 @@
         measures_transform_map_node.inputs.input_file = measures_list
         pan_workflow.connect(measures_transform_map_node,'out_file',roimean_map_node,'input_file')
             
     else:
         roimean_map_node.inputs.input_file = measures_list
 
 
-    if lesioncreate_node:
-        pan_workflow.connect(lesioncreate_node,'atlas_file',roimean_map_node,'lesion_file')
+    if maskcreate_node:
+        pan_workflow.connect(maskcreate_node,'atlas_file',roimean_map_node,'mask_file')
+    elif mask_templates:
+        roimean_map_node.inputs.mask_file = mask_templates
+
 
 
     if createGraph:
          pan_workflow.write_graph(graph2use='flat')
 
 
     return pan_workflow
```

### Comparing `panpipelines-0.9.9/src/panpipelines/workflows/tensor_workflow.py` & `panpipelines-1.0.0/src/panpipelines/workflows/tensor_workflow.py`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.9/src/panpipelines/workflows/textmeasures_workflow.py` & `panpipelines-1.0.0/src/panpipelines/workflows/textmeasures_workflow.py`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.9/src/panpipelines/workflows/volmeasures_workflow.py` & `panpipelines-1.0.0/src/panpipelines/workflows/volmeasures_workflow.py`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.9/.gitignore` & `panpipelines-1.0.0/.gitignore`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.9/LICENSE` & `panpipelines-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.9/README.md` & `panpipelines-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.9/pyproject.toml` & `panpipelines-1.0.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.9/PKG-INFO` & `panpipelines-1.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: panpipelines
-Version: 0.9.9
+Version: 1.0.0
 Summary: MRI Processing Pipelines for PAN Healthy Minds for Life Study
 Project-URL: Homepage, https://github.com/MRIresearch/PANpipelines
 Project-URL: Bug Tracker, https://github.com/MRIresearch/PANpipelines/issues
 Author-email: Chidi Ugonna <chidiugonna@arizona.edu>
 License: MIT License
         
         Copyright (c) 2023 MRIresearch
```

