# thyroid_ml
## Analysis of dataset from thyroid pacients diagnosis - supervised learning algorithms

This project was done in collaboration with two other classmates for the class `Knowledge Engineering` and had the following objectives in mind:<br>

# Project Overview (from class directives):
The file data.csv is a version of an archive of thyroid diagnoses
obtained from the Garvan Institute, consisting of 6420 records from 1984 to
early 1987.  Each record looks like

	(29 attribute values), diagnoses, [record identification]

The attributes are given in order and separated by commas.  Unknown attribute
values are indicated by question marks.  The attributes are

	Attribute Name			Possible Values
	--------------			---------------
	age:				continuous.
	sex:				M, F.
	on thyroxine:			f, t.
	query on thyroxine:		f, t.
	on antithyroid medication:	f, t.
	sick:				f, t.
	pregnant:			f, t.
	thyroid surgery:		f, t.
	I131 treatment:			f, t.
	query hypothyroid:		f, t.
	query hyperthyroid:		f, t.
	lithium:			f, t.
	goitre:				f, t.
	tumor:				f, t.
	hypopituitary:			f, t.
	psych:				f, t.
	TSH measured:			f, t.
	TSH:				continuous.
	T3 measured:			f, t.
	T3:				continuous.
	TT4 measured:			f, t.
	TT4:				continuous.
	T4U measured:			f, t.
	T4U:				continuous.
	FTI measured:			f, t.
	FTI:				continuous.
	TBG measured:			f, t.
	TBG:				continuous.
	referral source:		WEST, STMW, SVHC, SVI, SVHD, other.

The diagnosis consists of a string of letters indicating diagnosed conditions.
A diagnosis "-" indicates no condition requiring comment.  A diagnosis of the
form "X|Y" is interpreted as "consistent with X, but more likely Y".  The
conditions are divided into groups where each group corresponds to a class of
comments.

		Letter	Diagnosis
		------	---------

	hyperthyroid conditions:

		A	hyperthyroid
		B	T3 toxic
		C	toxic goitre
		D	secondary toxic

	hypothyroid conditions:

		E	hypothyroid
		F	primary hypothyroid
		G	compensated hypothyroid
		H	secondary hypothyroid

	binding protein:

		I	increased binding protein
		J	decreased binding protein

	general health:

		K	concurrent non-thyroidal illness

	replacement therapy:

		L	consistent with replacement therapy
		M	underreplaced
		N	overreplaced

	antithyroid treatment:

		O	antithyroid drugs
		P	I131 treatment
		Q	surgery

	miscellaneous:

		R	discordant assay results
		S	elevated TBG
		T	elevated thyroid hormones

In experiments with an earlier version of this archive, decision trees were
derived for the most frequent classes of comments, namely

	hyperthyroid conditions (A, B, C, D)
	hypothyroid conditions (E, F, G, H)
	binding protein (I, J)
	general health (K)
	replacement therapy (L, M, N)
	discordant results (R)


The goals established were divided into 3 iterations:
O1.

    Students should provide the best possible classification models using whatever method covered in class [Remember: within each model, everything else being similar, the simplest configurations should be preferred]
    Classification should be according to 8 classes of the target variable "diagnoses": 6 indicated at the end of data.names the class '-', corresponding to no condition, and other diagnoses.

O2.

    Can we confidently predict the age of the subject given the other attributes?
    Can we confidently predict the sex of the subject given the other attributes?

O3.

    What are the most significant features in the best models obtained above (in O1 and O2)?

The results can be found in the [notebook_EC.ipynb](Jupiter Notebook) in the root of this project.
