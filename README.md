# madara
# Test de push
# Déclaration de CGenerateurRequeteFireStore

STFrom est une Structure
	collectionId est une chaîne
FIN

STSelect est une Structure
	fields est un tableau de STFieldPath
FIN

STFieldFilter_Str est une Structure
	field	est un STFieldPath
	op		est une chaîne
	value	est un STStringValue
FIN

STFilters_Str est une Structure
	fieldFilter est un STFieldFilter_Str
FIN

STCompositeFilter est une Structure
	filters	est un tableau de JSON
	op		est une chaîne
FIN

stSimpleFilter est une Structure
	fieldFilter	est un tableau de JSON
	op			est une chaîne
FIN

STWhereComposite est une Structure
	compositeFilter est un JSON
FIN

STWhere est une Structure
	fieldFilter est un JSON
FIN

STOrderBy est une Structure
	field		est un STFieldPath
	direction	est une chaîne
FIN

STTri est une Structure
	sChamp		est une chaîne
	eDirection	est une EDirectionTriFirestore
FIN

STFiltre est une Structure
	sChamp		est une chaîne
	eOperateur	est une EOperateurFirestore
	sValeur		est une chaîne
FIN

CGenerateurRequeteFireStore est une Classe
PRIVÉ
	m_tabListeChampsSelect	est un tableau de chaînes
	m_tabListeChampsTrier	est un tableau de STTri
	m_tabListeDesFiltres	est un tableau de STFiltre
	m_nValeurLimite			est un entier
	m_sUrl					est une string
	m_stHttpOption			est STHttpOption
	m_HttpClientReponse		est un restRéponse
FIN
