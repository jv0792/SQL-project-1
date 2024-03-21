--Categorical analysis
-- Calculate the percentage of sites participating in Patient Assistance Programs (PAP)
SELECT
  'PAP' AS Program,
  COUNT(*) AS TotalSites,
  COUNT(CASE WHEN Is_PAP_Site = 1 THEN 1 END) AS ParticipatingSites,
  (COUNT(CASE WHEN Is_PAP_Site = 1 THEN 1 END) * 100.0) / COUNT(*) AS Percentage
FROM
  COVID_Treatments;

 

-- Calculate the percentage of sites with Telehealth capabilities
SELECT
  'Telehealth' AS Capability,
  COUNT(*) AS TotalSites,
  COUNT(CASE WHEN Is_Telehealth_Site = 1 THEN 1 END) AS SitesWithTelehealth,
  (COUNT(CASE WHEN Is_Telehealth_Site = 1 THEN 1 END) * 100.0) / COUNT(*) AS Percentage
FROM
  COVID_Treatments;

-- Calculate the percentage of sites participating in Test to Treat program (T2T)
SELECT
  'T2T' AS Program,
  COUNT(*) AS TotalSites,
  COUNT(CASE WHEN Is_T2T_Site = 1 THEN 1 END) AS ParticipatingSites,
  (COUNT(CASE WHEN Is_T2T_Site = 1 THEN 1 END) * 100.0) / COUNT(*) AS Percentage
FROM
  COVID_Treatments;
