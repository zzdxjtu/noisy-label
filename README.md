# noisy-label
2020年3月7日
Co-teaching: Robust Training of Deep Neural Networks with Extremely Noisy Labels
code ：https://github.com/bhanML/Co-teachin
in each mini-batch data, each network selects its small-loss instances as the useful knowledge, and teaches such useful instances to its peer network for the further training.
There are two important questions for designing above Algorithm 1:
Q1. Why can sampling small-loss instances based on dynamic R(T) help us find clean instances?
Q2. Why do we need two networks and cross-update the parameters?
deep networks will learn clean and easy pattern in the initial epochs， R(T) is large at the start, and gradually become smaller , keep clean instances and drop the noisy labels before netwok memorize them.
To sum up, as the error from one network will not be directly transferred back itself, we can expect that our Co-teaching method can deal with heavier noise compared with the self-evolving one.




Co-Mining: Deep Face Recognition with Noisy Labels
code : http://www.cbsr.ia.ac.cn/users/xiaobowang/
• We identify the samples in noisy face recognition dataset as three parts, i.e., the noisy faces, the highconfidence clean faces and the clean faces.
• We propose a novel co-mining framework, which employs two peer networks to detect the noisy faces, exchanges the high-confidence clean faces and reweights the clean faces in a mini-batch fashion.
• We emphasize the open-set evaluation for face recognition and conduct extensive experiments on both synthetic and real-world benchmarks, which have verifiedthe effectiveness of our new approach over the state-of-the-art alternatives.
