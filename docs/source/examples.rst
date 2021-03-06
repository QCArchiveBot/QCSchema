Examples
========

Several examples of completed schema. As the input is duplicated in the output
the corresponding input of these schema are the input fields alone.
Effectively, this is all keys above the "provenance" field. For clarify all
array-based values have been truncated to four decimal places.

Water MP2 Energy
~~~~~~~~~~~~~~~~

.. code:: python

  {
    "schema_name": "qc_schema_output",
    "schema_version": 1,
    "molecule": {
      "geometry": [
        0.0,  0.0,    -0.1294,
        0.0, -1.4941,  1.0274,
        0.0,  1.4941,  1.0274
      ],
      "symbols": ["O", "H", "H"]
    },
    "driver": "energy",
    "model": {
      "method": "MP2",
      "basis": "cc-pVDZ"
    },
    "keywords": {},
    "provenance": {
      "creator": "QM Program",
      "version": "1.1",
      "routine": "module.json.run_json"
    },
    "return_result": -76.22836742810021,
    "success": true,
    "properties": {
      "calcinfo_nbasis": 24,
      "calcinfo_nmo": 24,
      "calcinfo_nalpha": 5,
      "calcinfo_nbeta": 5,
      "calcinfo_natom": 3,
      "return_energy": -76.22836742810021,
      "scf_one_electron_energy": -122.44534536383037,
      "scf_two_electron_energy": 37.62246494040059,
      "nuclear_repulsion_energy": 8.80146205625184,
      "scf_dipole_moment": [0.0, 0.0, 2.0954],
      "scf_iterations": 10,
      "scf_total_energy": -76.02141836717794,
      "mp2_same_spin_correlation_energy": -0.051980792916251864,
      "mp2_opposite_spin_correlation_energy": -0.15496826800602342,
      "mp2_singles_energy": 0.0,
      "mp2_doubles_energy": -0.20694906092226972,
      "mp2_total_correlation_energy": -0.20694906092226972,
      "mp2_total_energy": -76.22836742810021
    }
  }


Water HF Gradient
~~~~~~~~~~~~~~~~~~

.. code:: python

  {
    "schema_name": "qc_schema_output",
    "schema_version": 1,
    "molecule": {
      "geometry": [
        0.0,  0.0,    -0.1294,
        0.0, -1.4941,  1.0274,
        0.0,  1.4941,  1.0274
      ],
      "symbols": ["O", "H", "H"]
    },
    "driver": "gradient",
    "model": {
      "method": "HF",
      "basis": "cc-pVDZ"
    },
    "keywords": {},
    "provenance": {
      "creator": "QM Program",
      "version": "1.1",
      "routine": "module.json.run_json"
    },
    "return_result": [
      0.0,  0.0,    -0.0595,
      0.0, -0.0430,  0.0297,
      0.0,  0.0430,  0.0297
    ],
    "success": true,
    "properties": {
      "calcinfo_nbasis": 24,
      "calcinfo_nmo": 24,
      "calcinfo_nalpha": 5,
      "calcinfo_nbeta": 5,
      "calcinfo_natom": 3,
      "return_energy": -76.02141836717794,
      "scf_one_electron_energy": -122.44534536383044,
      "scf_two_electron_energy": 37.622464940400654,
      "nuclear_repulsion_energy": 8.80146205625184,
      "scf_dipole_moment": [0.0, 0.0, 2.0954],
      "scf_iterations": 10,
      "scf_total_energy": -76.02141836717794
    }
  }


