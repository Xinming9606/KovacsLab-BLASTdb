# 🔬 KovacsLab BLAST Databases

This repository provides BLAST databases for use in your sequence analyses.

## 📂 Using the Database on IBL Server

If you are using the IBL server, you can copy the database to your own directory:

```bash
cp -r /home/xuxm/KovacsLab-BLASTdb/ /path/to/your/home
```

## 🛠️ How to Create a Customized BLAST Database
To create your own BLAST database from a FASTA file:

```bash
micromamba activate blast #only in IBL server
makeblastdb -in /path/to/your/home/*.fasta -dbtype nucl -out Elongation_factor_Tu2
