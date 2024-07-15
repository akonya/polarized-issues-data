# Polarized Issues Dataset

## Data Summary

This data was generated via [Remesh](https://www.remesh.ai/approach/collective-dialogue) during a working session funded by the [Peacetech and Polarization Lab](https://kroc.nd.edu/research/peacetech-and-polarization-lab-ptap/) at the University of Notre Dame on June 25, 2024 during the “Deliberative Technologies and Peacebuilding in Polarized Contexts Workshop.” During the working session, multiple [collective dialogues](https://arxiv.org/pdf/2311.02242) were conducted with N300 representative samples of the US public recruited via [Prolific](https://www.prolific.com/). They each focused on a polarizing topic among the US public:

- [Foreign intervention](https://github.com/akonya/polarized-issues-data/tree/main/Foreign%20intervention)
- [Right to assemble](https://github.com/akonya/polarized-issues-data/tree/main/Right%20to%20assemble)
- [Campus protests](https://github.com/akonya/polarized-issues-data/tree/main/Campus%20protests)

## Data Structure
Raw and aggregate data is provided for each collective dialogue.

### Raw data
All participant-level demographic, response, and vote data:
- **[*]_binary.csv** is a table of all agreement votes. All votes are binary [agree or disagree]. The ID of the response voted on is _Thought ID_. The ID of the voter is _Participant ID_.
- **[*]_preference.csv** is a table of all pairwise preference votes.  Most are simple pair votes  -- choose [thought A or thought B] --  but it also includes votes for when a participant can’t decide: ie. [I’m not sure, I disagree with both, I agree with both]. 
- **[*]_verbatim_map.csv** is a table of all thoughts (verbatim particpant responses). It maps _Thought IDs_ to the _Thought Text_ it corresponds to, along with the ID of the participant who submitted the response.
- **[*]_participants.csv** is a table of all participants. It gives the demographic and poll data for each _participant ID_ along with some other stuff.

### Aggregate data 
Demographic segment-level aggregations of results: 
- **[*]_aggreagate.csv** is a table of all responses and answer options to all prompts and questions, and what fraction of each participant segment selected or agreed* with them. 

_*note: Aggregate results for ‘opinion ask’ question types include [inferences](https://openreview.net/pdf?id=tkxnRPkb_H) for missing agreement votes._


## Data License
The data is licensed under CC By 4.0: [https://creativecommons.org/licenses/by/4.0/](https://creativecommons.org/licenses/by/4.0/)
