SELECT 
CONCAT(a.prenom, ' ', a.nom) AS athlete, p.nom AS pays
FROM athlete a
JOIN pays p ON p.id_pays = a.id_pays
JOIN participation pa ON pa.id_athlete = a.id_athlete
LEFT JOIN run r ON r.id_athlete = a.id_athlete AND r.id_epreuve = pa.id_epreuve
WHERE r.id_run IS NULL;
