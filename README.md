# PowerBI_Projets-TheFurnitureCompany

_Introduction_

La littératie financière est une compétence essentielle à une gestion efficace des opérations d’une entreprise. En effet, disposer suffisamment de connaissances sur le plan financier permet aux dirigeants d’une société une prise de décision éclairée. Cependant, un projet conjoint réalisé en 2017 entre le département de Recherche et intelligence de marché de BDC et l’École de gestion Telfer de l’Université d’Ottawa a dévoilé que «[p]lus des deux tiers des propriétaires d'entreprise se considèrent informés en matière financière» (La Littératie Financière Chez Les Entrepreneurs et Les Propriétaires d’Entreprise Canadiens, 2017). Par conséquent, cette déclaration nous révèle qu’il peut être difficile pour environ un tiers d’entre eux à comprendre les états financiers. 

Plusieurs entreprises disposent d’un ERP comptable qui dispose des données relatives aux opérations financières. Au lieu des bilans et états des résultats conventionnels, il est possible de créer des tableaux de bord connectés à ces bases de données, afin de présenter l’information sous un nouvel angle. Le projet explore l’hypothèse suivante : la présentation des résultats financiers à l’aide d’un tableau de bord facilite l’interprétation de l’information et conséquemment rend plus accessible l’information financière. 


_Déploiement du Modèle_

Le déploiement du tableau de bord sur l’analyse financière de The Furniture Company ainsi que les lignes de code Dax et M se retrouvent sur le GitHub .

Le modèle fut réalisé à l’aide des données provenant du Finance Data Sample of Furniture Company de Kaggle. Ces données se présentent sous forme de 5 fichiers distincts (Balance Sheet .xlsx, Budget.xlsx, Chart of Accounts.xlsx, data.csv, Income Statement.xlsx). Sur un serveur indépendant, la version 2022 de Microsoft SQL Server Management Studio a été installée et les fichiers y ont été importé dans une base de données nommée Furniture Company. 
Par la suite, les données furent connectées à Power BI Destop. À l’aide de Power Query et du langage M, les données ont été transformées (voir Code/M queries). Des dimensions ont été créées à l'aide de code DAX pour générer les différents visuels (voir Code/Dax dim). 


_Visualisation des Résultats_ 

Le document TheFurnitureCompany_Report.pdf présente les visualisations des données de l’entreprise. Il est possible de consulter le fichier TheFurnitureCompanu.pbix pour avoir un aperçu. Cependant, il n’est pas possible de le rafraîchir puisqu’il n’est pas directement lié à la base de données. L’onglet FinancialStatement a été utilisé pour balancer les états financiers. En manipulant les filtres, il est possible de remarquer que certaines données de la source sont manquantes ou erronées, ce qui altère le résultat final du rapport. Généralement, le total du « Income Statement » devrait correspondre au « Current Period Profit ». 


_Enjeux_

La phase de déploiement du projet visait à créer un tableau de bord en utilisant des données provenant d’une entreprise en simulant que celles-ci provenaient d’un système ERP d’une entreprise. L'objectif était de présenter les résultats financiers sous un nouvel angle, offrant ainsi des visualisations claires et des indicateurs clés de performance qui permettent d’évaluer efficacement la situation financière.
Cependant, les résultats de cette phase ont été impactés par des données à la source manquantes et incohérentes. Malgré la qualité des KPI et des visuels produits à l’aide de l’outil Power BI, l'absence de données valides s’est avérée un véritable obstacle dans la possibilité de créer un outil qui permet de prendre des décisions éclairées.


_Recommandations_ 

Ce projet met en lumière l'importance de la qualité et de l'accessibilité des données pour toute analyse financière. En effet, l’indisponibilité des données via l’accès direct à l’ERP de l’entreprise représente un enjeu notable. Afin d'améliorer la situation, il est essentiel de revoir les processus de collecte, de gestion et d'intégration des données financières avant d’en faire l’extraction.
L'entreprise pourrait envisager une révision de ses méthodes de collecte de données. Par exemple, elle pourrait effectuer une analyse financière similaire à celle proposée dans l’onglet « FiancialStatement ». Par ailleurs, des ajustements dans la manière dont les informations sont enregistrées et stockées dans le système ERP sont nécessaires pour combler les lacunes rencontrées lors du projet.


_Conclusion_

En conclusion, l'hypothèse initiale est réfutée, puisqu’il a été démontré que l'importance de disposer de données fiables pour toute analyse financière est essentiel. Ce résultat offre une piste afin de réévaluer et d'améliorer les processus de collecte et de gestion des données financière des entreprises. Rendant ainsi possible aux gestionnaires de prendre une prise de décision plus éclairée. 


_Bibliographie_

La littératie financière chez les entrepreneurs et les propriétaires d’entreprise canadiens. (2017). https://www.bdc.ca/globalassets/digizuite/10542-litteratie-financiere-chez-entrepreneurs-proprietaires-entreprise-canadiens.pdf

XING, Z. (n.d.). Finance Data Sample of Furniture Company. www.kaggle.com. Retrieved September 26, 2023, from https://www.kaggle.com/datasets/zhoumeixing/finance-data-sample-of-furniture-company

