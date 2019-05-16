# bangalore-calliope
Calliope model, specific to a (illustrative) district in Bangalore, India.

For more information on the model structure and general use of Calliope, see [the documentation](https://calliope.readthedocs.io/en/stable/).

![Bangalore district map](bangalore_district.png)

This commit provides the model for the publication:

`B. Pickering, R. Choudhary. Mitigating risk in district-level energy investment decisions by scenario optimisation, In: Proceedings of the 4th IBPSA-England Conference BSO 2018, Emmanuel College, Cambridge, 2018`

If you use this model or work derived from it in an academic publication, please cite the above publication!

## Install

This paper ran on a release candidate of Calliope 0.6.0. To install, clone this repository, navigate into the cloned directory and create the 'calliope_BSO2018' conda environment:

```shell
$ conda env create -f requirements.yml
```

## Running models

The notebook 'Building and running the model' will guide you through building the model. As we use predefined clusters, this version of Calliope requires manually setting up the model with the full (mean demand) timeseries before editing the time dimension to match the typical days used in the modelling.

## Notes

* Native Calliope plotting will not work in most cases, due to the existence of the 'scenario' dimension.
* Since the release of Calliope 0.6.0 and subsequent releases (at the time of writing) up to 0.6.4, there have been improvements, including mathematical formulation inconsistencies. This model will be re-run once the scenario optimisation branch has been fully incorporated in a stable Calliope release.

## License

[![Creative Commons License](https://i.creativecommons.org/l/by-sa/4.0/88x31.png)](https://creativecommons.org/licenses/by-sa/4.0/)

This work is licensed under a [Creative Commons Attribution-ShareAlike 4.0 International License](http://creativecommons.org/licenses/by-sa/4.0/).