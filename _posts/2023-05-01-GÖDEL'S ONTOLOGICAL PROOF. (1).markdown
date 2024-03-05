---
layout: post
title:  "GÖDEL'S ONTOLOGICAL PROOF. (1)"
date:   2023-05-01
last_modified_at: 2023-05-01
categories: [PHILOSOPHY]
---

※ 논리학적으로는 양상논리 S5 공리체계(Modal logic S5-axiomatic system)를 사용하는 증명방법입니다.

Ax. : Axiom(공리)ㅡ어떤 계(system)안에서 증명없이 옳다고 받아들이기로 한 기본명제

Th. : Theorem(정리)ㅡ공리와 정의로부터 따라나오는 명제

Df. : Definition(정의)ㅡ기호(notation)에 대한 약속

P : Positive property (property of being positive)

□ : it is necessarily true that ~

◇ : it is possibly true that~

∀ : for all

∃ : exist

￢ : not

ψ : psi(싸이), φ : phi(파이) → 여기서는 모두 특정 개념을 이름

‍

Ax. 1. {P(φ)∧□∀x[φ(x)→ψ(x)]}→P(ψ)

Ax. 2. P(φ)→◊∃x[φ(x)]

Th. 1. p(φ)→◇∃x[φ(x)]

Df. 1. G(x) ⟺ ∀φ[P(φ)→φ(x)]

Ax. 3. P(G)Th. 2. ◇∃xG(x)

Df. 2. φ ess x ⟺ φ(x) ∧ ∀ψ{ψ(x) → □ ∀x[φ(x)→ψ(x)]}

Ax. 4. P(φ) → □ P(φ)Th. 3. G(x) → G ess x

Df. 3. E(x) ⟺ ∀φ [φ ess x → □ ∃x φ (x)]

Ax. 5. P(E)

Th. 4. □ ∃x G(x)+ (∃x(Gx∧￢∃y(Gy∧x≠y)) = Godlike(=G)를 만족하는 대상은 유일하다)
