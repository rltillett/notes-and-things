# Oxford Nanopore Minion Cost Considerations

Richard Tillett
NV INBRE Bioinformatics
Nevada Center for Bioinformatics

[Oxford Nanopore Technologies](https://nanoporetech.com) (ONT) sells a portable, real-time DNA sequencer, MinION, that is radically compact, plugs into your PC via USB 3.0, and is purportedly cheap. Is it cheap enough to use in a classroom setting as a credible sequencing device? This report doesn't attempt to speak much about the credibility of the deivce. Suffice to say, I wouldn't offer it for consideration if I thought it lacked merit. It isn't high-throughput enough to do dozens of quantitative RNA-seq samples like an Illumina is, but if you want rapid sequencing or sequencing of very long molecules, the device shines. I hope the info provided helps in cost determination.

## How much does it cost?
From [the MinION product page](https://nanoporetech.com/products/minion), (emphasis added):
> The MinION is commercially available, simply by paying a starter-pack fee of **$1,000**. The MinION starter pack includes materials you need to run initial sequencing experiments, including a MinION device, flow cells and kits, as well as membership of the Nanopore Community.

Here's what comes in that $1000 starter pack. For the new customer $1000 basic package, you'd get:

Basic Starter Pack | $1,000.00
--|--
Flow Cell Wash Kit | 1
MinION Sequencing Device | 1
Starter Pack Flow Cell (R9.4)  | 2
Control Expansion | 1
Library prep kits  | 1
"Enhanced support" | no

So, you get one sequencing device (all of the MinION's electronics and structure, basically), and two of its microfluidics/nanopore guts (the R9.4 flow cells). Those flow cells are the main consumable of a sequencing run. They contain the nanopore-embedded membranes and electrode sensors that are the sequencing mechanism of this device. They do have a limited shelf life (proteins, after all), but can be safely re-used in some circumstances (see the included wash kit). And you get two of them.

That pack also nets you one library prep kit, of which there are possibly 9 to choose from, depending on the specifics of the sequencing experiment and strategy. From one view are three main flavors of kit

* [DNA prep without PCR](https://store.nanoporetech.com/pcr-free-kits/)
* [DNA prep with PCR](https://store.nanoporetech.com/pcr-free-kits/)
* [RNA prep kits](https://store.nanoporetech.com/cdna-and-direct-rna/)

Or you might view the kits from whether they are "Rapid sequencing" or "Ligation Sequencing." Neither choice _requires_ PCR, so long as you have 400 ng or 1 µg DNA, respectively. And since the nanopores have the ability to do extremely long read lengths, the PCR yes/no question is less niche and worth considering for many types of experiments, as PCR amplification protocols/kits generally produce fragments smaller than the extreme lengths ONT can generate (30 kba is not rare, they claim to have gotten as high as 2 Mba).

### Any hidden costs? + Lab/IT requirements

As with the choice of kit, the exact experimental design will dictate at least one cost I don't think is included/reflected in the $1000 promo kit -- your DNA/RNA extraction kit. ONT doesn't exactly sell their own, and I think their system is compatible with plenty of the kits every mol bio lab uses, but I haven't nailed down recommendations for "best", or "ok, but change your elution buffer to ___", or "generally avoid xxx".

One other hidden cost, I think, is barcodes. If you will be multiplexing samples, you will have to buy a separate barcoding or barcoding-compatible kit.

The nanopore community site has a page listing the IT requirements (basically any recent Mac or Windows computer with a USB 3.0 plug), and the lab equipment/consumables associated with the various preps, all here [https://nanoporetech.com/community/lab-it-requirements](https://nanoporetech.com/community/lab-it-requirements).

## Re-use costs

### Flowcells

Flowcells start at $900, and have 512 nanopore channels, or possibly >800. Their product info makes a few different claims. You need to open the packaging, rehydrate, and do some QC on flowcells within 10 days of delivery. **Need to use within 8 weeks** for warranty.

### Individual kits
Individual library prep kits range from $450-$700. There are a lot of options, but if you're specifically interested in the ultra-long read lengths of ONT, you only have to think about the no-PCR kits, and whether/how to barcode+multiplex. Shelf-life claimed to be 90 days.

* [DNA prep without PCR](https://store.nanoporetech.com/pcr-free-kits/)
* [DNA prep with PCR](https://store.nanoporetech.com/pcr-free-kits/)
* [RNA prep kits](https://store.nanoporetech.com/cdna-and-direct-rna/)


## There's also a more expensive starter pack for some reason

They have another "starter pack" that's almost 5x as expensive, comes with 1 more kit, and 2 more flow cells. I'm not sure if it's a great value, unless you really want 3 months of enhanced support.

Enhanced | $4909.00
--- | ---
Flow Cell Wash Kit | 1
MinION Sequencing Device | 1
Starter Pack Flow Cell (R9.4) | 4
Control Expansion | 1
Library prep kits  | 2
"Enhanced support" | yes, 3 months
