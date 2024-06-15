![image](https://github.com/mdzubair9492/IBM-Quantum-Challenge-2024/assets/142826904/af05cc5f-d2a9-4925-a4db-5318f497a5d7)

<h2>Overview:</h2>

Here, I have included all the lab files and necessary extra files which we were needed in the ibm challenge 2024.
In lab 2 utils.py is need to upload in the same working directory .

In lab 3 there are 3 ipynb files , birds_dataset, vqe.py, transpile_parallel.py, params_0_list.py, opt_params_shallow_vqc.npy are needed to upload in the same working directory.

<h2>Common Issues and Answers:</h2>
Some common issues and answers while uploading the notebooks are,

<ol>
<li>Module Not Found:</li>
No module named 'package_name': `%pip install package_name`

   If you have issues instaling locally, try cloud platforms like Google Colab or qBraid.

<li>Lab-Specific IssuesM</li>

Lab 0
401 Client Error: Unauthorized
Run %set_env QXToken= in the Setup section of each lab, every time you restart a kernel or switch notebooks. Ensure no spaces after = and run before importing the grader. If already imported, restart the kernel, set the token, and then import the grader.

<li>Package Not Found: qc_grader</li>
Install with `%pip install git+https://github.com/qiskit-community/Quantum-Challenge-Grader.git --upgrade.`

Lab 2
Installing graphviz
pip install graphviz only installs the Python interface. `Install Graphviz from Graphviz Download`. For issues, use Google Colab, qBraid, or other cloud providers.

Lab 3

AI Transpiler
File Not Found: qiskit-ibm.json
Save your IBM Quantum token:
`QiskitRuntimeService.save_account(
    channel="ibm_quantum",
    token="<MY_IBM_QUANTUM_TOKEN>",
    set_as_default=True,
    overwrite=True,
)`

Qiskit Serverless
Package Version Issue
Ensure Python version is 3.10 or 3.11.
403 Error
Create a working directory for your files. Place transpile_parallel.py in a /transpile_parallel directory.

Lab 4

Ex6
Ensure test_shallow_VQC calls old_ansatz instead of ansatz to prevent index issues.

Ex7
TypeError: Object of type UnsetType is not JSON serializable
Set all options, including DD sequence_type for option_0, even if DD is disabled. Ensure the sequence type matches.

