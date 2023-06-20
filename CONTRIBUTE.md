## Option 1: 
Please send a link to a missing dataset to Jana (jana.zeller@student.kit.edu) and Pascal (pascal.friederich@kit.edu).
Or, if you have a new dataset, please send it to us along with a short description.

## Option 2: 
Click on the `branch` button and then click on the green `new branch` button.
Edit the molecules.md or materials.md file directly online in github. You can use the `preview` button in the top to get a preview of your markdown.

## Option 3: 
1. Fork the Project (`git pull https://github.com/aimat-lab/ChemMatData.git`)
2. Create your Dataset / Feature Branch (`git checkout -b feature/AmazingDataset`)
3. Add your dataset either to the `molecules.md` or `materials.md files`. You add a column to the table by adding a new line and entering each entry of the table. Different entries should be separated using `|`. One of your added datasets could for example look like this:
```
| PCQM4Mv2 | Quantum Mechanics | Based on the PubChemQC, we define a meaningful ML task of predicting DFT-calculated HOMO-LUMO energy gap of molecules given their 2D molecular graphs. The HOMO-LUMO gap is one of the most practically-relevant quantum chemical properties of molecules since it is related to reactivity, photoexcitation, and charge transport. | 1 | 3,378,606 | `Regression` | SMILES | [website](https://ogb.stanford.edu/docs/lsc/pcqm4mv2/#dataset) | |
```
4. Commit your Changes (`git commit -m 'Add some AmazingDataset'`)
5. Push to the Branch (`git push origin feature/AmazingDataset`)
6. Open a Pull Request. You open a pull request by clicking on the branch icon in the start page and navigating to the branch you just added. In the yellow banner click the `Compare & pull request` button. Select the `main` branch as the branch you want to merge into. Write a short description about the dataset you added. Then click on `Create Pull Request`. See [this full detailed description](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/creating-a-pull-request) from GitHub on how to open pull requests.


