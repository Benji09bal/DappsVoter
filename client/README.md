Le composant ContractBtns fournit les actions suivantes :

addVoter: Ajoute un électeur en utilisant l'adresse spécifiée.
addProposal: Ajoute une proposition en utilisant la description spécifiée.
vote: Effectue un vote pour une proposition en utilisant l'ID spécifié.
startProposalsRegistration: Démarre l'enregistrement des propositions.
endProposalsRegistration: Termine l'enregistrement des propositions.
startVotingSession: Démarre la session de vote.
endVotingSession: Termine la session de vote.
tallyVotes: Effectue le dépouillement des votes.
addWhitelist: Ajoute un électeur à la liste blanche en utilisant l'adresse spécifiée.
getWinningProposalID: Récupère l'ID de la proposition gagnante.
getVoter: Récupère les informations d'un électeur en utilisant l'adresse spécifiée.
getOneProposal: Récupère les informations d'une proposition en utilisant l'ID spécifié.
Détails du Composant

Le composant Contract est un composant fonctionnel qui utilise les hooks useState et useEffect de React. Il initialise le contrat et récupère des données à partir de celui-ci.

Initialisation
La fonction initContract est appelée lorsque le composant est monté. Elle initialise la bibliothèque Web3 et récupère le contrat de vote. Le code d'exemple montre comment initialiser Web3 en utilisant MetaMask. Vous pouvez modifier ce code pour correspondre à votre cas d'utilisation spécifique.

Récupération de Données
La fonction fetchData est appelée lorsque l'objet de contrat est défini. Elle récupère l'identifiant de la proposition gagnante à partir du contrat en utilisant la méthode winningProposalID. La valeur récupérée est stockée dans l'état value.

Rendu
Le composant affiche un message de chargement lorsque l'objet de contrat est nul. Une fois que l'objet de contrat est défini, il affiche les informations du contrat, telles que le titre du contrat.

Licence

Ce composant est publié sous la licence MIT. N'hésitez pas à le modifier et à l'utiliser dans vos projets.