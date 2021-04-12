# # Note 1

SLAM

L'objectif est de se positionner dans un milieu inconnu est grace a de mutliple observation, se localiser dans ce milieu ainsi que de trouver les reperes

Notation mathematique:
$$
x_k = \text{Position du Robot au temps k [Vector]} \\
u_k = \text{Deplacement du Robot du temps k-1 a k [Vector]} \\
m_i = \text{Repere i (fixe dans le temps) [Vector])} \\
z_{ik} = \text{Observation du repere i au temps k [Vector]} \\
z_{k} = \text{Liste des observation de repere au temps k [Vector]} \\
X_{0:k} = \text{Historiques des position } x \text{ [List[Vector]]} \\
U_{0:k} = \text{Historiques des deplacements } u \text{ [List[Vector]]} \\
m = \text{La liste de tout les repere [List[Vector]]} \\
Z_{0:k} = \text{Historique La liste de toutes les objervation } z_{k} \text{[List[List[Vector]]]}
$$


Le but du slam est determiner ceci:
$$
P(x_k, m| Z_{0:k}, U_{0:k}, x_0)
$$
