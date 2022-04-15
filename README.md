# divarizky
SELECT 
	npm, nama, nilai, 
	if (nilai > 78, "lulus", "tidak luls") As keterangan 
	FROM mhs1;

SELECT
 npm, nama, nilai,
 if (nilai <=50, "tidak lulus", "lulus") as keterangan
 FROM `mhs1`;

SELECT
npm,nama,nilai,
IF(nilai >= 80, "A",
IF(nilai >= 70 && nilai < 80, "B",
IF(nilai >= 60 && nilai < 70, "C",
IF(nilai >= 50 && nilai < 60, "D", "E")))) AS Grade,
IF(nilai >= 60, "lulus", "tidak lulus")
FROM mhs1; 
