<div>
<img src="resources/egfr-diagram.png" style="width:40%;height:auto"/>
<img src="resources/kholo-gel.png" style="width:40%;height:auto"/>
</div>

<span style="font-size:0.75em">
Kholodenko BN, [**Journal of Biological Chemistry**](http://www.jbc.org/content/274/42/30169.short) (1999)</span>

note:
    In our lab, we develop technology to support standards in model development.
    To put this talk in context, the types of models we support are kinetic models, usually of molecular processes. An example would be this EGFR pathway shown here, which is an autocrine signaling pathway that is mutated in the majority of cancers, hence it is a target for detailed study. To construct a model like this, you first start with prior knowledge of all the pathway steps. In this pathway, the ligand epidermal growth factor binds to its receptor on the cell surface, and then the bound complex is internalized. Next, it interacts with a bunch of adapter proteins and eventually activates its downstream effector ERK, a kinase which regulates many genes related to growth in the cell. You can write out an on rate and an off rate for each of these steps, which results in a system of ordinary differential equations. However, you will typically not know the values of the on rates and off rates themselves, instead you will have some sort of data like this. This data is basically quantifying a Western blot of phospho-tyrosine, which is a stand-in for activated EGF receptor, vs total EGF receptor, so it should in theory give a picture of how much of the receptor is activated. You can use this data to fit the on and off constants. This model is kind of overparameterized for the amount of data here, but its also a 20 year-old model. As the data improves so does the predictivity of the model.
    ERK: (extracellular signal–regulated kinases).
