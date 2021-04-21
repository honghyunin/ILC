

# 대칭키 암호화

``동일한 키로 암호화와 복호화를 동시에 할 수 있는 방식입니다.``

예를 들어 '가나다라'라는 키로 암호화를 하면, 복호화 시에 '가나다라'를 입력해주어야 합니다. 위 과정에서는 대칭키 전달 과정에서 누군가가 대칭키를 획득한다면 쉽게 암호화된 데이터를 알아낼 수 있습니다.

하지만 위 과정에선 대칭키 전달 과정에서 ``누군가가 대칭키를 획득한다면`` **쉽게 암호화된 데이터를 알아낼 수 있습니다.**

<br>

# 공개키 방식

- 지정된 인증기관에 의해 제공되는 키 값이다.

<br>

# 공개키 방식

공개키 방식에서는 두 개의 키를 갖습니다. 누구에가나 공개가 가능한 **공개키**, 자신만이 갖고 있는 **개인키(비공개 키, 비밀키)**.

이 공개키 알고리즘은 공개키로 암호화를 하냐, 개인키로 암호화를 하냐에 따라 사용분야가 달라집니다.

- 공개키로 암호화를 하면 데이터 보안에 중점을 두고,
- 개인키로 암호화를 하면 인증 과정에 중점을 두는 것입니다.

<br>

# 공개키로 암호화를 하는 경우

상대방의 공개키로 데이터를 암호화하고 데이터를 전달하면, 데이터를 전달받은 사람은 자신의 개인키로 데이터를 복호화합니다.

- A키로 암호화를 한다면, B키로 복호화하가 가능하고,
- B키로 암호화를 한다면, A키로 복호화가 가능한 것입니다.

- 이 공개키 방식 원리의 이해를 돕기 위한 예시를 들어보겠습니다.

``연인 사이인 두 사람이 다른 사람 몰래 편지를 주고받기로 하고 자물쇠가 달려있는 작은 상자와 이를 열 수 있는 열쇠를 각자 하나씩 가지고 있다고 가정해 보겠습니다. 두 사람은 서로에게 보낼 편지를 써서 상자에 넣은 후 자물쇠를 잠그고 보낸다면 열쇠를 가지고 있는 두 사람만이 비밀편지를 볼 수 있겠죠? 중간에 누군가가 상자를 가로챈다고 하더라도 열쇠를 가진 두 사람 이외에는 누구도 상자를 열어볼 수 없기 때문에 비밀편지 내용은 누설되지 않게 될 것입니다.

<br>

# 개인키로 암호화를 하는 경우(전자서명)

- 개인키의 소유자가 개인키로 데이터를 암호화하고 공개키와 함께 전달합니다. 이 과정에서 공개키와 데이터를 획득한 사람은 공개키를 이용하여 복호화가 가능합니다. 이런 위험에도 불구하고 이 방법을 사용하는 이유는 데이터 보호의 목적보다는 공개키가 데이터 제공자의 신원을 보장해주기 때문입니다. **``암호화된 데이터가 공개키로 복호화된다는 것은 공개키와 쌍을 이루는 개인키에 의하여 암호화되었다는 것을 의미합니다. 즉 데이터 제공자의 신원 확인이 보장된다는 것입니다.``**
