# Comparing `tmp/PACMAN-charge-0.1.2.tar.gz` & `tmp/PACMAN-charge-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PACMAN-charge-0.1.2.tar", last modified: Wed May  1 03:57:51 2024, max compression
+gzip compressed data, was "PACMAN-charge-0.1.3.tar", last modified: Sat May  4 13:24:03 2024, max compression
```

## Comparing `PACMAN-charge-0.1.2.tar` & `PACMAN-charge-0.1.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-01 03:57:51.774957 PACMAN-charge-0.1.2/
--rwxrwxrwx   0 root         (0) root         (0)     1068 2024-03-25 02:54:44.000000 PACMAN-charge-0.1.2/LICENSE
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-01 03:57:51.655310 PACMAN-charge-0.1.2/PACMANCharge/
--rwxrwxrwx   0 root         (0) root         (0)       33 2024-04-29 12:12:36.000000 PACMAN-charge-0.1.2/PACMANCharge/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)    28392 2024-01-10 01:22:23.000000 PACMAN-charge-0.1.2/PACMANCharge/atom_init.json
--rwxrwxrwx   0 root         (0) root         (0)    28219 2024-05-01 03:57:35.000000 PACMAN-charge-0.1.2/PACMANCharge/pmcharge.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-01 03:57:51.719309 PACMAN-charge-0.1.2/PACMAN_charge.egg-info/
--rwxrwxrwx   0 root         (0) root         (0)     3306 2024-05-01 03:57:51.000000 PACMAN-charge-0.1.2/PACMAN_charge.egg-info/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)      334 2024-05-01 03:57:51.000000 PACMAN-charge-0.1.2/PACMAN_charge.egg-info/SOURCES.txt
--rwxrwxrwx   0 root         (0) root         (0)        1 2024-05-01 03:57:51.000000 PACMAN-charge-0.1.2/PACMAN_charge.egg-info/dependency_links.txt
--rwxrwxrwx   0 root         (0) root         (0)      121 2024-05-01 03:57:51.000000 PACMAN-charge-0.1.2/PACMAN_charge.egg-info/requires.txt
--rwxrwxrwx   0 root         (0) root         (0)       18 2024-05-01 03:57:51.000000 PACMAN-charge-0.1.2/PACMAN_charge.egg-info/top_level.txt
--rwxrwxrwx   0 root         (0) root         (0)     3306 2024-05-01 03:57:51.772955 PACMAN-charge-0.1.2/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)     2918 2024-05-01 02:30:46.000000 PACMAN-charge-0.1.2/README.md
--rwxrwxrwx   0 root         (0) root         (0)       38 2024-05-01 03:57:51.775956 PACMAN-charge-0.1.2/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     1038 2024-05-01 03:57:40.000000 PACMAN-charge-0.1.2/setup.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-01 03:57:51.757310 PACMAN-charge-0.1.2/test/
--rwxrwxrwx   0 root         (0) root         (0)    34098 2024-05-01 02:36:11.000000 PACMAN-charge-0.1.2/test/Cu-BTC.cif
--rwxrwxrwx   0 root         (0) root         (0)        0 2024-03-25 03:31:56.000000 PACMAN-charge-0.1.2/test/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)       76 2024-05-01 02:36:03.000000 PACMAN-charge-0.1.2/test/test.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-04 13:24:03.528351 PACMAN-charge-0.1.3/
+-rwxrwxrwx   0 root         (0) root         (0)     1068 2024-03-25 02:54:44.000000 PACMAN-charge-0.1.3/LICENSE
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-04 13:24:03.358302 PACMAN-charge-0.1.3/PACMANCharge/
+-rwxrwxrwx   0 root         (0) root         (0)       33 2024-04-29 12:12:36.000000 PACMAN-charge-0.1.3/PACMANCharge/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)    28392 2024-01-10 01:22:23.000000 PACMAN-charge-0.1.3/PACMANCharge/atom_init.json
+-rwxrwxrwx   0 root         (0) root         (0)    26400 2024-05-04 13:21:02.000000 PACMAN-charge-0.1.3/PACMANCharge/pmcharge.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-04 13:24:03.424300 PACMAN-charge-0.1.3/PACMAN_charge.egg-info/
+-rwxrwxrwx   0 root         (0) root         (0)     3306 2024-05-04 13:24:03.000000 PACMAN-charge-0.1.3/PACMAN_charge.egg-info/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)      334 2024-05-04 13:24:03.000000 PACMAN-charge-0.1.3/PACMAN_charge.egg-info/SOURCES.txt
+-rwxrwxrwx   0 root         (0) root         (0)        1 2024-05-04 13:24:03.000000 PACMAN-charge-0.1.3/PACMAN_charge.egg-info/dependency_links.txt
+-rwxrwxrwx   0 root         (0) root         (0)      121 2024-05-04 13:24:03.000000 PACMAN-charge-0.1.3/PACMAN_charge.egg-info/requires.txt
+-rwxrwxrwx   0 root         (0) root         (0)       18 2024-05-04 13:24:03.000000 PACMAN-charge-0.1.3/PACMAN_charge.egg-info/top_level.txt
+-rwxrwxrwx   0 root         (0) root         (0)     3306 2024-05-04 13:24:03.526350 PACMAN-charge-0.1.3/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)     2918 2024-05-01 02:30:46.000000 PACMAN-charge-0.1.3/README.md
+-rwxrwxrwx   0 root         (0) root         (0)       38 2024-05-04 13:24:03.529350 PACMAN-charge-0.1.3/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     1038 2024-05-04 13:15:18.000000 PACMAN-charge-0.1.3/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-04 13:24:03.511350 PACMAN-charge-0.1.3/test/
+-rwxrwxrwx   0 root         (0) root         (0)    34098 2024-05-01 02:36:11.000000 PACMAN-charge-0.1.3/test/Cu-BTC.cif
+-rwxrwxrwx   0 root         (0) root         (0)        0 2024-03-25 03:31:56.000000 PACMAN-charge-0.1.3/test/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)       76 2024-05-01 02:36:03.000000 PACMAN-charge-0.1.3/test/test.py
```

### Comparing `PACMAN-charge-0.1.2/LICENSE` & `PACMAN-charge-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `PACMAN-charge-0.1.2/PACMANCharge/atom_init.json` & `PACMAN-charge-0.1.3/PACMANCharge/atom_init.json`

 * *Files identical despite different names*

### Comparing `PACMAN-charge-0.1.2/PACMANCharge/pmcharge.py` & `PACMAN-charge-0.1.3/PACMANCharge/pmcharge.py`

 * *Files 6% similar despite different names*

```diff
@@ -99,15 +99,14 @@
         idx_sorted = np.argsort(n_distance[idx_i])[: 200]
         _nonmax_idx.append(idx_i[idx_sorted])
     _nonmax_idx = np.concatenate(_nonmax_idx)
     index1 = _c_index[_nonmax_idx]
     index2 = _n_index[_nonmax_idx]
     dij = n_distance[_nonmax_idx]
     numbers = []
-    # s_data = mg.Structure.from_file(mof)
     try:
         elements = [str(site.specie) for site in struct.sites]
     except:
         elements = [str(site.species) for site in struct.sites]
     for i in range(len(elements)):
         ele = elements[i]
         atom_index = periodic_table_symbols.index(ele)
@@ -143,23 +142,22 @@
                 structure.get_structures()
         coords = structure.frac_coords
         try:
             elements = [str(site.specie) for site in structure.sites]
         except:
             elements = [str(site.species) for site in structure.sites]
         pos = []
-        lattice = structure.lattice.matrix
         for i in range(len(elements)):
             x = coords[i][0]
             y = coords[i][1]
             z = coords[i][2]
             pos.append([float(x),float(y),float(z)])
     except Exception as e:
         print(e)
-    return lattice, pos
+    return pos
 
 def average_and_replace(numbers, di):
     groups = defaultdict(list)
     for i, number in enumerate(numbers):
         if di ==3:
             key = format(number, '.3f')
             groups[key].append(i)
@@ -249,38 +247,35 @@
 
 def collate_pool(dataset_list):
     batch_atom_fea = [] 
     batch_nbr_fea =[]
     batch_nbr_fea_idx1 = []
     batch_nbr_fea_idx2 = []
     batch_num_nbr = []
-    batch_cell_atoms =[]
-    batch_cell_crys = []
     crystal_atom_idx = []
     batch_pos = []
     batch_dij_ = []
     base_idx = 0
-    for i, ((atom_fea, nbr_fea, nbr_fea_idx1, nbr_fea_idx2, num_nbr, dij_), (pos,cell_atoms,cell_crys))\
+    for i, ((atom_fea, nbr_fea, nbr_fea_idx1, nbr_fea_idx2, num_nbr, dij_), (pos))\
         in enumerate(dataset_list):       
         n_i = atom_fea.shape[0]
         batch_atom_fea.append(atom_fea)
         batch_nbr_fea.append(nbr_fea);batch_dij_.append(dij_)
         tt1 = np.array(nbr_fea_idx1)+base_idx
         tt2 = np.array(nbr_fea_idx2)+base_idx
         batch_nbr_fea_idx1.append(torch.LongTensor(tt1.tolist()))
         batch_nbr_fea_idx2.append(torch.LongTensor(tt2.tolist()))
         batch_num_nbr.append(num_nbr)
         crystal_atom_idx.append(torch.LongTensor([i]*n_i))
-        batch_cell_atoms.append(cell_atoms); batch_cell_crys.append(cell_crys)
         batch_pos.append(pos)
         base_idx += n_i
     return (torch.cat(batch_atom_fea, dim=0),torch.cat(batch_nbr_fea, dim=0),
             torch.cat(batch_nbr_fea_idx1, dim=0),torch.cat(batch_nbr_fea_idx2, dim=0),
             torch.cat(batch_num_nbr, dim=0),torch.cat(crystal_atom_idx,dim=0), torch.cat(batch_dij_,dim=0),
-            torch.cat(batch_pos,dim=0), torch.cat(batch_cell_atoms,dim=0), torch.cat(batch_cell_crys))
+            torch.cat(batch_pos,dim=0))
             
 class GaussianDistance(object):
     def __init__(self, dmin, dmax, step, var=None):
         assert dmin < dmax
         assert dmax - dmin > step
         self.filter = np.arange(dmin, dmax+step, step)
         if var is None:
@@ -314,46 +309,40 @@
 				super(AtomCustomJSONInitializer, self).__init__(atom_types)
 				for key in range(101):
 						zz = np.zeros((101,))
 						zz[key] = 1.0
 						self._embedding[key] = zz.reshape(1,-1)
     
 class CIFData(Dataset):
-    def __init__(self,crystal_data,pos,cell,radius,dmin,step):
+    def __init__(self,crystal_data,pos,radius,dmin,step):
         self.pos = pos
-        self.cell = cell
         self.radius = radius
         self.crystal_data = crystal_data
         atom_init_file = resource_filename('PACMANCharge', 'atom_init.json')
         self.ari = AtomCustomJSONInitializer(atom_init_file)
         self.gdf = GaussianDistance(dmin=dmin, dmax=self.radius, step=step)
     def __len__(self):
         return 1
     @functools.lru_cache(maxsize=None) 
     def __getitem__(self,_):
         nums = self.crystal_data['numbers']
         atom_fea = np.vstack([self.ari.get_atom_fea(nn) for nn in nums])
         pos = self.pos
-        cell = self.cell.reshape(1,9)
-        cell_repeat = np.repeat(cell[0,0:9].reshape(1,9),len(nums),axis=0)
         index1 = np.array(self.crystal_data['index1'])
         nbr_fea_idx = np.array(self.crystal_data['index2'])
         dij = np.array(self.crystal_data['dij']); dij_ = torch.Tensor(dij)
         nbr_fea = self.gdf.expand(dij)
         num_nbr = np.array(self.crystal_data['nn_num'])
         atom_fea = torch.Tensor(atom_fea)
         nbr_fea = torch.Tensor(nbr_fea)
         nbr_fea_idx1 = torch.LongTensor(index1)
         nbr_fea_idx2 = torch.LongTensor(nbr_fea_idx)
         num_nbr = torch.Tensor(num_nbr)
         pos = torch.Tensor(pos)
-        cell = np.copy(cell)
-        cell_crys = torch.Tensor(cell)
-        cell_atoms = torch.Tensor(cell_repeat)
-        return (atom_fea, nbr_fea, nbr_fea_idx1, nbr_fea_idx2, num_nbr,dij_), (pos,cell_atoms,cell_crys)
+        return (atom_fea, nbr_fea, nbr_fea_idx1, nbr_fea_idx2, num_nbr,dij_), (pos)
     
 class Normalizer(object):
 	def __init__(self, tensor):
 		self.mean = torch.mean(tensor)
 		self.std = torch.std(tensor)
 	def norm(self, tensor):
 		return (tensor - self.mean) / self.std
@@ -406,47 +395,43 @@
     def __init__(self,orig_atom_fea_len,nbr_fea_len,atom_fea_len,n_conv,n_feature):    
         super(SemiFullGN, self).__init__()
         self.node_embedding = nn.Linear(orig_atom_fea_len,atom_fea_len)
         self.edge_embedding = nn.Linear(nbr_fea_len,atom_fea_len)
         self.convs = nn.ModuleList([ConvLayer(atom_fea_len=atom_fea_len,nbr_fea_len=atom_fea_len) for _ in range(n_conv)])
         self.feature_embedding = nn.Sequential(nn.Linear(n_feature,512))
         self.atom_nbr_fea_embedding = nn.Sequential(nn.Linear(2*atom_fea_len,128))
-        self.cell_embedding = nn.Sequential(nn.Linear(9,128))
         self.phi_pos = nn.Sequential(nn.Linear(512+128+128,512),
                                      nn.BatchNorm1d(512),
                                      nn.LeakyReLU(0.2))
         self.conv = nn.Sequential(nn.Conv1d(64,512,3,stride=1,padding=0),nn.BatchNorm1d(512),nn.LeakyReLU(0.2),
                                    nn.Conv1d(512,512,3,stride=1,padding=0),nn.BatchNorm1d(512),nn.LeakyReLU(0.2),
                                    nn.Conv1d(512,256,3,stride=1,padding=1),nn.LeakyReLU(0.2),
                                    nn.Conv1d(256,256,3,stride=1,padding=1),nn.LeakyReLU(0.2),
                                    nn.Conv1d(256,1,kernel_size=4,stride=1,padding=0))
-    def forward(self,atom_fea,nbr_fea,nbr_fea_idx1,nbr_fea_idx2,num_nbrs,atom_idx,structure_feature,cell):
+    def forward(self,atom_fea,nbr_fea,nbr_fea_idx1,nbr_fea_idx2,num_nbrs,atom_idx,structure_feature):
         nbr_fea_idx1 = nbr_fea_idx1.cuda() if torch.cuda.is_available() else nbr_fea_idx1
         nbr_fea_idx2 = nbr_fea_idx2.cuda() if torch.cuda.is_available() else nbr_fea_idx2
         num_nbrs = num_nbrs.cuda() if torch.cuda.is_available() else num_nbrs
         atom_idx = atom_idx.cuda() if torch.cuda.is_available() else atom_idx
         atom_fea = atom_fea.cuda() if torch.cuda.is_available() else atom_fea
         nbr_fea = nbr_fea.cuda() if torch.cuda.is_available() else nbr_fea 
         structure_feature = structure_feature.cuda() if torch.cuda.is_available() else structure_feature
-        cell = cell.cuda() if torch.cuda.is_available() else cell
         atom_fea = self.node_embedding(atom_fea)
         nbr_fea = self.edge_embedding(nbr_fea)
         N,_ = atom_fea.shape 
         for conv_func in self.convs:
             nbr_fea,atom_fea,_,atom_nbr_fea = conv_func(atom_fea,nbr_fea,nbr_fea_idx1,nbr_fea_idx2,num_nbrs,atom_idx)
         feature = structure_feature[atom_idx]
-        cell = cell[atom_idx]
         feature = self.feature_embedding(feature)
         atom_nbr_fea = self.atom_nbr_fea_embedding(atom_nbr_fea)
-        cell = self.cell_embedding(cell)
-        final_feature = torch.cat((atom_nbr_fea,cell,feature),dim=-1)
-        ddec = self.phi_pos(final_feature)
-        ddec = ddec.view(N,64,8)
-        ddec = self.conv(ddec).squeeze()
-        return ddec
+        final_feature = torch.cat((atom_nbr_fea,feature),dim=-1)
+        charge = self.phi_pos(final_feature)
+        charge = charge.view(N,64,8)
+        charge = self.conv(charge).squeeze()
+        return charge
     
 class ConvLayerE(nn.Module):
     def __init__(self,atom_fea_len,nbr_fea_len):
         super(ConvLayerE,self).__init__()
         self.atom_fea_len = atom_fea_len
         self.nbr_fea_len = nbr_fea_len
         self.tanh_e = nn.Tanh()
@@ -480,19 +465,19 @@
         atom_nbr_fea = torch.cat([vi,ek_sum],dim=1)
         global_fea = Variable(torch.zeros((Ncrys,2*M)).cuda() if torch.cuda.is_available() else torch.zeros((Ncrys,2*M)) ).scatter_add(0,crystal_atom_idx.view(-1,1).repeat(1,2*M),atom_nbr_fea)
         return ek,vi,global_fea
     
 class GCN(nn.Module):
     def __init__(self,orig_atom_fea_len,nbr_fea_len,atom_fea_len,n_conv,n_feature):    
         super(GCN, self).__init__()
-        self.node_embedding = nn.Linear(orig_atom_fea_len,atom_fea_len)
-        self.edge_embedding = nn.Linear(nbr_fea_len,atom_fea_len)
-        self.convs = nn.ModuleList([ConvLayerE(atom_fea_len=atom_fea_len,nbr_fea_len=atom_fea_len) for _ in range(n_conv)])
-        self.phi_u = nn.Sequential(nn.Linear(2*atom_fea_len,n_feature),nn.LeakyReLU(0.2),
-				   nn.Linear(n_feature,n_feature),nn.Tanh())
+        self.node_embedding = nn.Linear(orig_atom_fea_len,atom_fea_len).to(device)
+        self.edge_embedding = nn.Linear(nbr_fea_len,atom_fea_len).to(device)
+        self.convs = nn.ModuleList([ConvLayerE(atom_fea_len=atom_fea_len,nbr_fea_len=atom_fea_len).to(device) for _ in range(n_conv)])
+        self.phi_u = nn.Sequential(nn.Linear(2*atom_fea_len,n_feature).to(device),nn.LeakyReLU(0.2).to(device),
+				   nn.Linear(n_feature,n_feature).to(device),nn.Tanh().to(device))
     def Encoding(self,atom_fea,nbr_fea,nbr_fea_idx1,nbr_fea_idx2,num_nbrs,crystal_atom_idx):
         nbr_fea_idx1 = nbr_fea_idx1.cuda() if torch.cuda.is_available() else nbr_fea_idx1
         nbr_fea_idx2 = nbr_fea_idx2.cuda() if torch.cuda.is_available() else nbr_fea_idx2
         num_nbrs = num_nbrs.cuda() if torch.cuda.is_available() else num_nbrs
         crystal_atom_idx = crystal_atom_idx.cuda() if torch.cuda.is_available() else crystal_atom_idx
         atom_fea = atom_fea.cuda() if torch.cuda.is_available() else atom_fea
         nbr_fea = nbr_fea.cuda() if torch.cuda.is_available() else nbr_fea 
@@ -541,63 +526,43 @@
     print(f"Digits: {digits}")
     print(f"Atom Type: {atom_type}")
     print(f"Neutral: {neutral}")
 
     try:
         struc = ase_format(cif_file)
         crystal_data = CIF2json(struc,cif_file)
-        cell,pos=pre4pre(cif_file)
-        dataset = CIFData(crystal_data,pos,cell,6,0,0.2)
+        pos=pre4pre(cif_file)
+        dataset = CIFData(crystal_data,pos,6,0,0.2)
         loader= get_data_loader(dataset=dataset, batch_size=1, num_workers=0, collate_fn=collate_pool, pin_memory=False)
         for batch in loader:
             chg_1 = batch[0].shape[-1]+3
             chg_2 = batch[1].shape[-1]
             orig_atom_fea_len = batch[0].shape[-1]
         gcn = GCN(orig_atom_fea_len, chg_2, 128, 7, 256) 
         gcn.to(device)
         chkpt_ddec = torch.load(charge_model_name, map_location=torch.device(device))
         model4chg = SemiFullGN(chg_1,chg_2,128,8,256)
         model4chg.cuda() if torch.cuda.is_available() else model4chg.to(device)
         model4chg.load_state_dict(chkpt_ddec['state_dict'])
         model4chg.eval()
         for _, (input) in enumerate(loader):
             with torch.no_grad():
-                if device == "cuda":
-                    input_cuda = [input_tensor.to(device) for input_tensor in input]
-                    input_var = (input_cuda[0].cuda(),
-                                    input_cuda[1].cuda(),
-                                    input_cuda[2].cuda(),
-                                    input_cuda[3].cuda(),
-                                    input_cuda[4].cuda(),
-                                    input_cuda[5].cuda())
-                    encoder_feature = gcn.Encoding(*input_var)
-                    atoms_fea = torch.cat((input_cuda[0],input_cuda[7]),dim=-1)
-                    input_var2 = (atoms_fea.cuda(),
-                                    input_cuda[1].cuda(),
-                                    input_cuda[2].cuda(),
-                                    input_cuda[3].cuda(),
-                                    input_cuda[4].cuda(),
-                                    input_cuda[5].cuda(),
-                                    encoder_feature.cuda(),
-                                    input_cuda[9][:,:9].cuda())
-                else:
-                    input_var = (input[0],
-                                    input[1],
-                                    input[2],
-                                    input[3],
-                                    input[4],
-                                    input[5])
-                    encoder_feature = gcn.Encoding(*input_var)
-                    atoms_fea = torch.cat((input[0],input[7]),dim=-1)
-                    input_var2 = (atoms_fea,
-                                    input[1],
-                                    input[2],
-                                    input[3],
-                                    input[4],
-                                    input[5],
-                                    encoder_feature,
-                                    input[9][:,:9])
+                input_var = (input[0].to(device),
+                                input[1].to(device),
+                                input[2].to(device),
+                                input[3].to(device),
+                                input[4].to(device),
+                                input[5].to(device))
+                encoder_feature = gcn.Encoding(*input_var)
+                atoms_fea = torch.cat((input[0],input[7]),dim=-1)
+                input_var2 = (atoms_fea.to(device),
+                                input[1].to(device),
+                                input[2].to(device),
+                                input[3].to(device),
+                                input[4].to(device),
+                                input[5].to(device),
+                                encoder_feature.to(device))
                 chg = model4chg(*input_var2)
                 chg = charge_nor.denorm(chg.data.cpu())
                 write4cif(cif_file,chg,digits=digits,atom_type=atom_type,neutral=neutral,charge_type=charge_type)
     except Exception as e:
         print(e)
```

### Comparing `PACMAN-charge-0.1.2/PACMAN_charge.egg-info/PKG-INFO` & `PACMAN-charge-0.1.3/PACMAN_charge.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PACMAN-charge
-Version: 0.1.2
+Version: 0.1.3
 Summary: Partial Atomic Charges for Porous Materials based on Graph Convolutional Neural Network (PACMAN)
 Home-page: https://github.com/sxm13/PACMAN
 Author: Guobin Zhao
 Author-email: sxmzhaogb@gmai.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `PACMAN-charge-0.1.2/PKG-INFO` & `PACMAN-charge-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PACMAN-charge
-Version: 0.1.2
+Version: 0.1.3
 Summary: Partial Atomic Charges for Porous Materials based on Graph Convolutional Neural Network (PACMAN)
 Home-page: https://github.com/sxm13/PACMAN
 Author: Guobin Zhao
 Author-email: sxmzhaogb@gmai.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `PACMAN-charge-0.1.2/README.md` & `PACMAN-charge-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `PACMAN-charge-0.1.2/setup.py` & `PACMAN-charge-0.1.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import requests
 from setuptools import setup, find_packages
 
 setup(
     name="PACMAN-charge",
-    version="0.1.2",
+    version="0.1.3",
     packages=find_packages(),
     description="Partial Atomic Charges for Porous Materials based on Graph Convolutional Neural Network (PACMAN)",
     author="Guobin Zhao",
     author_email="sxmzhaogb@gmai.com",
     url="https://github.com/sxm13/PACMAN",
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
```

### Comparing `PACMAN-charge-0.1.2/test/Cu-BTC.cif` & `PACMAN-charge-0.1.3/test/Cu-BTC.cif`

 * *Files identical despite different names*

