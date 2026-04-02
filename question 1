SELECT a.nom, a.prenom, e.nom AS epreuve,
SUM(n.valeur * c.poids) / SUM(c.poids) AS note_finale
FROM athlete a
JOIN run r ON r.id_athlete = a.id_athlete
JOIN epreuve e ON e.id_epreuve = r.id_epreuve
JOIN note n ON n.id_run = r.id_run
JOIN critere c ON c.id_critere = n.id_critere
GROUP BY a.id_athlete, a.nom, a.prenom, e.id_epreuve, e.nom
ORDER BY e.nom, note_finale DESC;

