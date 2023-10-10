# Taste Retargeting via Chemical Taste Modulators
This is the repository for the hardware schematics and compounds used in the "Taste Retargeting via Chemical Taste Modulators" paper (ACM UIST 2023). Thank you to [Alex Mazursky](https://www.alexmazursky.com/) for his help with the hardware design.

[Paper](https://lab.plopes.org/published/2023-UIST-TasteRetargeting-AuthorCopy.pdf)

**Original Paper Abstract:** Prior research has explored modifying taste through electrical stimulation. While promising, such interfaces often only elicit taste changes while in contact with the user’s tongue (e.g., cutlery with electrodes), making them incompatible with eating and swallowing real foods. Moreover, most interfaces cannot selectively alter basic tastes, but only the entire flavor profile (e.g., cannot selectively alter bitterness). To tackle this, we propose taste retargeting, a method of altering taste perception by delivering chemical modulators to the mouth before eating. These modulators temporarily change the response of taste receptors to foods, selectively suppressing or altering basic tastes. Our first study identified six accessible taste modulators that suppress salty, umami, sweet, or bitter and transform sour into sweet. Using these findings, we demonstrated an interactive application of this technique with the example of virtual reality, which we validated in our second study. We found that taste retargeting reduced the flavor mismatch between a food prop and other virtual foods.

## Modulators covered in paper
We propose interactively delivering taste modulators to alter taste perception while eating or drinking. However, given the lack of prior work in using taste modulators for interactive experiences, we had to identify and characterize a set of modulators that were accessible to realize our concept. Thus, we provide an overview of our modulators, including toxicological information. We specifically opted for easier access modulators (e.g., food safe, supplement, off-the-shelf, etc.), leading to modulators with suppressing or transforming effects. However, other modulators exist (e.g., demonstrated in mice or prescription medications) that might act as enhancers, which we discuss in Future Work.

### Gymnemic acids: sweet suppressor
Gymnema acids allows us to achieve sweet suppression. This is a chemical isolated from the leaves of Gymnema sylvestre. This leaf powder is a commonly available as a dietary supplement and thus food-safe; ours was purchased from Best Naturals. We use a concentration of 1.0% w/v based on Okamoto et al. [54].
Taste alteration mechanism: Of our chosen modulators, this may be the most well-known, second only to miraculin. This sweet suppression has been attributed to its triterpene glycosides [5, 74]. More recently, Sanematsu et al. found that these gymnemic acids bind to the human sweet taste receptor hT1R3 to produce its sweet-suppressing effect [64].

### Clofibric acid: sweet and umami suppressor
Clofibric acid allows us to achieve simultaneous sweet & umami suppression. Clofibric acid (PubChem CID: 2797, Catalog #: 21608) was purchased from Cayman Chemical Company at its highest available purity (≥98%). We use a dose of 51.45 mg, based on Kochem & Breslin [33], well below its acute oral toxicity (LD50) of 897 mg/kg [90].
Taste alteration mechanism: Clofibric acid has been shown to be an antagonist for the sweet taste receptor (hT1R2-hT1R3), which also contributes to umami perception. In other words, clofibric acid binds and inhibits this receptor’s activity. This inhibition diminishes sweet and umami perception in humans [33, 34, 40].

### Lactisole: sweet and umami suppressor
Lactisole (PubChem CID: 16231, Catalog #: 18657) was purchased from Cayman Chemical Company at its highest available purity (≥98%). We use a dose of approximately 3.75 mg, based on Sclafani and Pérez [68]. This modulator is approved for use in foods at levels up to 150 ppm (approximately 150 mg) per food item [9]. Lactisole is a commonly used sweet modulator in industrial food processing [68]. The food industry typically uses lactisole to avoid perceiving an increase in sweetness when additional sugar is introduced for texture-purposes (e.g., softness).
Taste alteration mechanism: Lactisole achieves its sweet and umami suppression by blocking the activation of the hT1R2-hT1R3 receptor [33, 34].

### Miraculin: sweet modulator
Miracle berry tablets are a commonly available food supplement derived from berries (Synsepalum dulcificum, known as “miracle fruit”). We source ours from the off-the-shelf product mberry. We use 200 mg of miracle berry dissolved in water. The key active ingredient, miraculin, produces the taste alteration. Miraculin is not associated with any safety concerns and does not represent a risk of allergy or toxicity to humans [76].
Taste alteration mechanism: Of our modulators, miraculin is the most recognizable as it is commercially advertised as a “party trick” [16]. Miraculin binds to human sweet taste receptor hT1R2-hT1R3. While miraculin acts as an inhibitor at neutral pH environments, it functions as a strong agonist in the presence of acidic pH environments [36]. In other words, miraculin causes acidic stimuli to activate a sweet taste receptor. This is why it is used as a “party trick” with acidic foods, such as making a lemon taste sweet. In addition, the perceived sourness of acidic stimuli is diminished, with mostly the sweet signal reaching the primary taste area [86]. The exact mechanism of miraculin interaction with taste receptors remains unknown. However, miraculin interacts with lactisole, with psychophysical findings showing that lactisole diminishes the pH-dependent sweet response produced by miraculin [24, 36].

### Zinc sulfate: sweet & bitter suppressor
Zinc sulfate (PubChem CID: 24424) is a chemical commonly available in food supplements and has the U.S. Food and Drug Administration’s “Generally Regarded as Safe” status for food and beverages. We source it from an off-the-shelf product by Triquetra Health. We use a dose of 4 mg derived from pilots. Zinc sulfate’s acute oral toxicity (LD50) is 1,538 mg/kg.
Taste alteration mechanism: Zinc sulfate is a sweet inhibitor [27, 28] and selective bitter inhibitor [29]. The exact mechanisms by which zinc ions affect sweet and bitter taste are still unknown, but Keast et al. suggests that they bind to taste receptors, altering their binding properties [27].

Since publishing the paper, we identified that Ionic Zinc's bitterness actually comes from another compound in the mixture, notably copper sulfate. We recommend experimenting with tablets that are largely zinc sulfate, such as Windmill or Puregen Labs Zinc Sulfate tablets, which are available on Amazon.

#### Amiloride: salty suppressor
Amiloride (PubChem CID: 16231, Catalog #: 14409) was purchased from Cayman Chemical Company at its highest available purity (≥98%). We use a dose of 1.722 mg, based on Schiffman et al.’s [65]. This modulator’s acute oral toxicity (LD50) of this modulator is 300 mg/kg [89].
Taste alteration mechanism: Amiloride has been used as a specific inhibitor of sodium transport (reducing saltiness). The psychophysical findings that amiloride reduces the intensity of taste perception of sodium and lithium salts is consistent with its action in which the fluxes of sodium and lithium are molecularly blocked [65].


## Citation
When using or building upon this work **in an academic publication**, please consider citing our paper:

Jas Brooks, Noor Amin, and Pedro Lopes. 2023. “Taste Retargeting via Chemical Taste Modulators.” In Proceedings of ACM Symposium on User Interface Software and Technology 2023 (UIST ’23). Association for Computing Machinery, New York, NY, USA. DOI:10.1145/3586183.3606818
