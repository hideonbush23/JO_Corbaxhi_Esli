SELECT 
CONCAT(a.prenom, ' ', a.nom) AS athlete,
COUNT(p.id_epreuve) AS nb_epreuves
FROM athlete a
JOIN participation p ON p.id_athlete = a.id_athlete
GROUP BY a.id_athlete, a.nom, a.prenom
HAVING COUNT(p.id_epreuve) >= 2;
