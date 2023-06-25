## Option 1: 
Please send a link to a missing dataset to Jana (jana.zeller@student.kit.edu) and Pascal (pascal.friederich@kit.edu).
Or, if you have a new dataset, please send it to us along with a short description.

## Option 2: 
Click on the `branch` button and then click on the green `new branch` button.
Edit the `molecules.json` or `materials.json` file directly online in github.

## Option 3: 
1. Fork the Project (`git pull https://github.com/aimat-lab/ChemMatData.git`)
2. Create your Dataset / Feature Branch (`git checkout -b feature/AmazingDataset`)
3. Open the desired JSON file (molecules.json or materials.json) in a text editor.
4. Create a new JSON object that represents your dataset. Make sure to include all the relevant fields: Dataset Name, Domain, Task Type, Data Type, #Compounds, #Tasks, Short Description, Papers, and DownloadLink.
5. If the dataset has multiple values for Task Type, Data Type, or DownloadLink, separate each entry with a comma followed by a whitespace (", ").
6. For the Papers field, create an array of objects where each object represents a paper with the fields Name and Link.

Your JSON could now look like this:
```
{
    "Dataset Name": "QM9",
    "Domain": "Quantum Mechanics",
    "Short Description": "QM9 is a comprehensive dataset that provides geometric, energetic, electronic and thermodynamic properties for a subset of GDB-17 database, comprising 134 thousand stable organic molecules with up to nine heavy atoms. All molecules are modeled using density functional theory (B3LYP/6-31G(2df,p) based DFT)",
    "#Tasks": 16,
    "#Compounds": 134000,
    "Task Type": "Regression",
    "Data Type": "SMILES, 3D coordinates",
    "DownloadLink": "http://quantum-machine.org/datasets/#:~:text=Available%20via-,figshare,-.",
    "Papers" : [
        {
            "Name": "Enumeration of 166 billion organic small molecules in the chemical universe database GDB-17",
            "Link": "http://pubs.acs.org/doi/abs/10.1021/ci300415d"
        },
        {
            "Name": "Quantum chemistry structures and properties of 134 kilo molecules",
            "Link": "http://quantum-machine.org/datasets/#:~:text=A.%20von%20Lilienfeld%2C-,Quantum%20chemistry%20structures%20and%20properties%20of%20134%20kilo%20molecules,-%2C%20Scientific%20Data"
        }
    ]
}
```
7. Add your new dataset object to the array, making sure to place a comma before it.
8. Commit your Changes (`git commit -m 'Add some AmazingDataset'`)
9. Push to the Branch (`git push origin feature/AmazingDataset`)
10. Open a Pull Request. You open a pull request by clicking on the branch icon in the start page and navigating to the branch you just added. In the yellow banner click the `Compare & pull request` button. Select the `main` branch as the branch you want to merge into. Write a short description about the dataset you added. Then click on `Create Pull Request`. See [this full detailed description](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/creating-a-pull-request) from GitHub on how to open pull requests.


