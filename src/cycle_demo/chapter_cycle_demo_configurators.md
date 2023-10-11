# Product Configurators

We are going to Explain and show how the configurator works based on two examples:

1. bicycle configurator
2. unicycle configurator

First a step by step guide on how to set up a product configurator:

1. Enable the product configurator extension in Nvidia Omniverse

2. Create a "configurators" folder

3. Download the following requirements which the extension is going to use and paste them into the "configurators" folder:
    - link to DataStructure
    - link to Assets
    - link to empty configurator scene

4. Open the empty configurator scene in Omniverse Usd-Composer

5. Add a reference to your product you would like to configure under the ConfigurableAssets Scope Folder
    - You can download our product_P3_bicycle or product_P2_unicycle if you like
    - If you use your own: your products must contain variant sets and variants for the configurator to work

6. In Tools/Product Configurator/Utilities select "Create DataStructure"
    - The first input field needs the path to the DataStructure/Prims folder.
    - The second input field needs the path to the DataStructure/Graphs folder.
    - Click on create and the necessary files and action graphs for the extension to work will be generated

7.  Now we need to enable the actual change between different variations in our product:
    - In the Stage window find the Graphs Scope Folder
    - Search for every Graph which starts with "variantController"
    - Unfold it and search for the set_variant_selection_01 prim
    - In the property window --> mark "Set Variant" as true

8. Open the Configurator Panel with Tools/Product Configurator/Panel

9. If you wish you can download our configurator_P3_basicbike or configurator_P2_unicycle

That is all it takes to make the configurator work.