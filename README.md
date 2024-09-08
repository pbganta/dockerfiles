# dockerfiles
Docker files to create images that contain popular python packages such as Scikit-learn, Atomic Simulation Environment (ASE) and MDAnalysis. ASE and MDAnalysis facilitates molecular simulations analysis and Scikit-learn enables application of ML algorithms.

To run script inputfile.py, go to folder with inputfile.py and run below command:

docker run --rm --name c_ase -it --mount type=bind,source="$(pwd)",target=/app  ase_mdanalysis_scikit:1.0

Then execute ls to find the files in your folder. Run python3 inputfile.py to do analysis with ASE, MDAnalysis or Scikit-learn. 
