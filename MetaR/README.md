![MetaR logo](images/MetaR-logo-4-SMALL-300x111.png)

MetaR takes advantage of Language Workbench Technology to facilitate data analysis with the R language. It can be used by:

* biologists with limited computational experience. No programming skills are required to start analyzing data.
* bioinformaticians who need to perform repetitive analyses and find it beneficial to design and use specialized analyses micro-languages to increase productivity and consistency of data analysis.
* bioinformaticians who wish to package state of the art analysis methods into user friendly metaR analysis language constructs. MetaR can act as a bridge between analysis experts who develop analysis methods in R and wish to distribute these methods to the broadest audience without investing a lot of effort in developing user interfaces.

MetaR is designed to work well with other languages of the platform. Importantly, users who learn how to use one component will acquire skills useful with other languages offered on the platform.

The following snapshot illustrates how metaR simplifies data analysis: we call differentially expressed genes with edgeR, join the resulting table with the table of counts, and produce a heatmap for the top 5% differentially regulated genes:
 
![MetaR snapshot](images/MetaR_Home_Snapshot.png){:height="60%" width="60%"}

Here’s another example showing how to look at intersection of gene lists with the integration of UpSetR/MetaR integration:

![MetaR snapshot2](images/UpSet_in_MetaR_Snapshot.png){:height="60%" width="60%"}

## Installation 

MetaR can be installed on the following platforms:
* MacOS Sierra 10.12+
* 64bit Windows 10 Pro, Enterprise and Education (1607 Anniversary Update, Build 14393 or later)
* Any Linux distribution supporting Java 8 (check here for a complete list)

To install MetaR, see installation instructions for each supported platform: 

[Installation instructions for MacOS users](macos/README.md).

Installation instructions for Windows users (TBP).

Installation instructions for Linux users (TBP).

## Upgrade
To upgrade MetaR, use the MPS&gt;Preferences...&gt;Plugins dialog. MPS will notify you of available upgrades. Follow instructions to install the new version of the plugin.

## Documentation
The following documentation booklet provides a comprehensive documentation about how to use and contribute to MetaR:
 * [MetaR booklet (pdf)](booklet/MetaR_booklet.pdf)


## Source code
MetaR is available on its [GitHub repository](https://github.com/manuelesimi/MetaR).

MetaR is currently in active development: please use the GitHub issue tracker to file enhancement requests and bug fixing.

## Releases and change log
See MetaR [releases](https://github.com/manuelesimi/MetaR/releases) on GitHub.

## License
MetaR is open-source and released under the [Apache 2.0 license](http://www.apache.org/licenses/LICENSE-2.0).

## Citation

If you use MetaR, please cite:

Fabien Campagne, William ER Digan, Manuele Simi _MetaR: simple, high-level languages for data analysis with the R ecosystem_ bioRxiv 2015 doi: http://dx.doi.org/10.1101/030254