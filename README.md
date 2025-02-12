# cricket-catalase-rnai
These data files and code are associated with the scientific article 
"Tissue- and temperature-dependent expression, enzyme activity, and RNAi knockdown of Catalase in a freeze-tolerant insects."<br>
This material is under the same copyright protections as the article itself.

# RCode file
The code can be run in R v4.0.3, and was used to conduct statistical analysis and generate the manuscript figures from the data files below. (Recommendation: use RStudio for easier visualization of figures.)


# Data files
These are used for statistical analysis and figure generation in the RCode file.

## Acclimation_EnzymeActivity_forR.csv
This reports Catalase enzyme activity for crickets exposed to different durations of fall-like acclimation conditions
Each row pertains to a different pool of tissues from 3 crickets, with information provided for each variable (column heading), as described below.

VARIABLE:                         DESCRIPTION <br>
#Tissue:                          Type of tissue: FB (fat body), MG (midgut), or MT (Malpighian tubules)br>
#SampleID:                        Unique sample identifier<br>
#AcclimationTime:                 Duration of acclimation exposure in weeks<br>
#CatalaseActivity(U/mgProtein):   Catalase enzyme activity, expressed in units per mg protein in the tissue<br>
#RelativeCatalase_Activity:       Ratio of catalase enzyme activity in each sample relative to the average of 0 weeks acclimated crickets for that tissue<br>

## Acclimation_qPCR_forR.csv
This reports relative Catalase mRNA abundance for crickets exposed to different durations of fall-like acclimation conditions
Each row pertains to a different pool of tissues from 3 crickets, with information provided for each variable (column heading), as described below.

VARIABLE:                         DESCRIPTION <br>
#Tissue:                          Type of tissue: FB (fat body), MG (midgut), or MT (Malpighian tubules)br>
#AcclimationTime:                 Duration of acclimation exposure in weeks<br>
#SampleID:                        Unique sample identifier<br>
#ef1:                             Cq (also know as Ct) value for the reference gene, ef1<br>
#cat:                             Cq (also know as Ct) value for the target gene, catalase<br>
#DeltaCq:                         Difference in Cq values between target and reference gene (cat - ef1)<br>
#DeltaDeltaCq:                    Difference in DeltaCq values between each sample and the relevant mean Delta Cq value for control samples (0 weeks acclimated)<br>
#RelativeCatalase_mRNA:           Abundance of catalse mRNA in each sample relative to the control for that tissue and experiment (2^-DeltaDeltaCq)<br>

## RNAi_EnzymeActivity_AllTissues_forR.csv
This reports Catalase enzyme activity for unacclimated crickets exposed to different RNAi treatments.
Each row pertains to a different cricket, with information provided for each variable (column heading), as described below.

VARIABLE:                         DESCRIPTION <br>
#Tissue:                          Type of tissue: FB (fat body), MG (midgut), or MT (Malpighian tubules)br>
#SampleID:                        Unique sample identifier<br>
#AssayWeek:                       Date on which injections were performed<br>
#Treatment:                       Whether the cricket was injected with dsRNA targeting Catalase (RNAi) or a vehicle control (Control)<br>
#RNAi_Temp:                       Temperature at which crickets were maintained post-injection until tissues were dissected for enzyme assays<br>
#RNAi_Days:                       Time in days for which crickets were maintained post-injection until tissues were dissected for enzyme assays<br>
#CatalaseActivity(U/mgProtein):   Catalase enzyme activity, expressed in units per mg protein in the tissue<br>
#RelativeCatalase_Activity:       Ratio of catalase enzyme activity in each sample relative to the average of 0 weeks acclimated crickets for that tissue<br>

## RNAi_EnzymeActivity_Temperature_forR.csv
This reports Catalase enzyme activity for acclimated crickets exposed to different RNAi treatments.
Each row pertains to a different cricket, with information provided for each variable (column heading), as described below.

VARIABLE:                         DESCRIPTION <br>
#Tissue:                          Type of tissue: FB (fat body) or MG (midgut)<br>
#SampleID:                        Unique sample identifier<br>
#AssayWeek:                       Date on which injections were performed<br>
#Treatment:                       Whether the cricket was injected with dsRNA targeting Catalase (RNAi) or a control construct (Control)<br>
#RNAi_Condition:                  A description of the combined temperature and time described in the next two columns<br>
#RNAi_Temp:                       Temperature at which crickets were maintained post-injection until tissues were dissected for enzyme assays<br>
#RNAi_Days:                       Time in days for which crickets were maintained post-injection until tissues were dissected for enzyme assays<br>
#CatalaseActivity(U/mgProtein):   Catalase enzyme activity, expressed in units per mg protein in the tissue<br>
#RelativeCatalase_Activity:       Ratio of catalase enzyme activity in each sample relative to the average of 0 weeks acclimated crickets for that tissue<br>

## RNAi_qPCR_AllTissues_forR.csv
This reports relative Catalase mRNA abundance for for unacclimated crickets exposed to different RNAi treatments.
Each row pertains to a different cricket, with information provided for each variable (column heading), as described below.

VARIABLE:                         DESCRIPTION <br>
#Tissue:                          Type of tissue: FB (fat body), MG (midgut), or MT (Malpighian tubules)br>
#AcclimationTime:                 Duration of acclimation exposure in weeks<br>
#SampleID:                        Unique sample identifier<br>
#AssayWeek:                       Date on which injections were performed<br>
#Treatment:                       Whether the cricket was injected with dsRNA targeting Catalase (RNAi) or a vehicle control (Control)<br>
#RNAi_Temp:                       Temperature at which crickets were maintained post-injection until tissues were dissected for enzyme assays<br>
#RNAi_Days:                       Time in days for which crickets were maintained post-injection until tissues were dissected for enzyme assays<br>
#ef1:                             Cq (also know as Ct) value for the reference gene, ef1<br>
#cat:                             Cq (also know as Ct) value for the target gene, catalase<br>
#DeltaCq:                         Difference in Cq values between target and reference gene (cat - ef1)<br>
#DeltaDeltaCq:                    Difference in DeltaCq values between each sample and the relevant mean Delta Cq value for control samples (Control)<br>
#RelativeCatalase_mRNA:           Abundance of catalse mRNA in each sample relative to the control for that tissue and experiment (2^-DeltaDeltaCq)<br>

## RNAi_qPCR_Temperature_forR.csv
This reports Catalase enzyme activity for acclimated crickets exposed to different RNAi treatments.
Each row pertains to a different cricket, with information provided for each variable (column heading), as described below.

VARIABLE:                         DESCRIPTION <br>
#Tissue:                          Type of tissue: FB (fat body) or MG (midgut)<br>
#SampleID:                        Unique sample identifier<br>
#AssayGroup:                      Cohort of crickets on which injections were performed<br>
#Treatment:                       Whether the cricket was injected with dsRNA targeting Catalase (RNAi) or a control construct (Control)<br>
#RNAi_Condition:                  A description of the combined temperature and time described in the next two columns<br>
#RNAi_Temp:                       Temperature at which crickets were maintained post-injection until tissues were dissected for enzyme assays<br>
#RNAi_Days:                       Time in days for which crickets were maintained post-injection until tissues were dissected for enzyme assays<br>
#ef1:                             Cq (also know as Ct) value for the reference gene, ef1<br>
#cat:                             Cq (also know as Ct) value for the target gene, catalase<br>
#DeltaCq:                         Difference in Cq values between target and reference gene (cat - ef1)<br>
#DeltaDeltaCq:                    Difference in DeltaCq values between each sample and the relevant mean Delta Cq value for control samples (Control)<br>
#RelativeCatalase_mRNA:           Abundance of catalse mRNA in each sample relative to the control for that tissue and experiment (2^-DeltaDeltaCq)<br>

## SurvivalRNAi_forR.csv
Survival of acclimated crickets following RNAi and a moderate freeze treament (1.5h at -8C).
Each row pertains to a different group of crickets, with information provided for each variable (column heading), as described below.

VARIABLE:                  DESCRIPTION <br>
#Treatment:                Whether crickets were injected with a dsRNA targeting catalase (RNAi) or a control construct (Control) prior to the freeze treatment<br>
#Alive:                    Number of crickets that were alive post-freeze<br>
#Dead:                     Number of crickets that were dead post-freeze<br>
#PAlive:                   Proportion of crickets that were alive post-freeze<br>
#SEP:                      Standard error of proportion of living crickets<br>
