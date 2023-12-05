This folder contais:
1) NMRcnstr.py: This script will display the NMR constrains used for a structure calculation atop a structure
2) Dyana.pdb: The coordinates of a peptide structure calculated with Dyana.
3) Dyana.upl: The constrains used for the structure calculation by Dyana.
4) cns.pdb: The coordinates of a peptide calculated with X-PLOR
5) cns.tbl: The constrains used for the structure calculation by X-PLOR
6) README.txt: This file.

A)	First open pymol. 
	Then change the path to the directory where you have extracted this files. For example: 
	PyMOL>cd c:\show_NMR_constraints

B) 	Load the pdb molecule structure. For example Dyana.pdb or cns.pdb

C) 	and type:
	PyMOL>run NMRcnstr.py

D)	Then type:
	upl('Dyana.upl') or cns('cns.tbl')

you will see the constrains as dashes on top of 20 NMR ensemble structures. 
If you have an ensemble of structures, you may move through the structures or play them as a movie if you type:

	PyMOL>mplay




NOTES: 	a)This is a very preliminary version. The scripts do not represent correctly the pseudoatom constrains, especially for the X-PLOR. While for the DYANA case there is a slight problem with the explicitly assigned instead of pseudoatoms. The scripts will be modified to correctly assimilate them soon.
	b) For the X-PLOR case be carefull how to represent the constraints. Look the example. They must be one constraint per line and separated like the example.




