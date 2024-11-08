# [🗺️ SeoulPOT 🗺️](http://15.165.46.156/)

<details>
  <summary><h2>🖥️ 2nd-agile</h2></summary>
  <p><strong>개발 기간</strong> | 2024-08-28 ~ 2024-09-27 (총 30일)</p>
  <p><strong>개발 목표</strong> | 웹 UI 개선, 기능 성능 강화, 데이터 분석 수행, 데이터 업데이트 자동화</p>
  <p><strong>UI</strong> |</p>
<table style="width: 100%; border-collapse: collapse;">
  <tr>
    <th align="center">
      한글 UI
    </th>
    <th align="center">
      영어 UI
    </th>
  </tr>
  <tr>
    <td align="center">
      <img src="https://github.com/user-attachments/assets/ccbe19ee-93f0-4c89-be38-7d8e6e08d094" width="500"/>
    </td>
    <td align="center">
      <img src="https://github.com/user-attachments/assets/665f4684-3119-434b-a127-4bf05501c25a" width="500"/>
    </td>
  </tr>
  <tr>
    <td align="center">
      <img src="https://github.com/user-attachments/assets/cc9283ac-1be0-483b-b132-4734506c325b" width="500"/>
    </td>
    <td align="center">
      <img src="https://github.com/user-attachments/assets/d9071641-c327-4d13-a929-633a072af297" width="500"/>
    </td>
  </tr>
  
  <tr>
    <td align="center">
      <img src="https://github.com/user-attachments/assets/cbf38bb9-5502-4d06-b055-0ccd3866e3a9" width="500"/>
    </td>
    <td align="center">
      <img src="https://github.com/user-attachments/assets/0d370d5b-569a-4553-bfc1-23bb0dc65173" width="500"/>
    </td>
  </tr>
  <tr>
    <td align="center">
      <img src="https://github.com/user-attachments/assets/375bf580-65c7-4f43-82ab-7b839da39059" width="500"/>
    </td>
    <td align="center">
      <img src="https://github.com/user-attachments/assets/213e3fb4-9f94-406d-92c5-3828e871420e" width="500"/>
    </td>
  </tr>
  <tr>
    <td align="center">
      <img src="https://github.com/user-attachments/assets/02ed4d4e-7d51-4d24-bb57-09ef4223a556" width="500"/>
    </td>
    <td align="center">
      <img src="https://github.com/user-attachments/assets/4ec75489-ea10-498b-8fab-fa9dbe0fa9b7" width="500"/>
    </td>
  </tr>
  <tr>
    <td align="center">
      <img src="https://github.com/user-attachments/assets/588fe046-52e9-44c8-9c53-7add02ae7fd6" width="500"/>
    </td>
    <td align="center">
      <img src="https://github.com/user-attachments/assets/63904072-988c-4e8b-b653-8242e6b3a7c1" width="500"/>
    </td>
  </tr>
</table>



</details>

<details>
  <summary><h2>🗂️ 요구사항 정의서</h2></summary>
  <details>
    <summary>프로젝트 관리</summary>
    <br/>
    <img src="https://github.com/user-attachments/assets/93ce529c-6a90-4bdd-b278-1b404907bfa5"  width="700"/>
  </details>
  <details>
    <summary>웹</summary>
    <br/>
    <img src="https://github.com/user-attachments/assets/d386f944-154c-4a11-940a-864fbf9fbf34"  width="700"/>
  </details>
  <details>
    <summary>DA-AI</summary>
    <br/>
    <img src="https://github.com/user-attachments/assets/e5405161-76f5-4746-912b-26c5891bccee"  width="700"/>
  </details>
  <details>
    <summary>DE</summary>
    <br/>
    <img src="https://github.com/user-attachments/assets/fa0537cc-bf91-4233-a98a-1bd4a9d4cbbe"  width="700"/>
  </details>
</details>

<details>
  <summary><h2>🎨 Figma</h2></summary>
  <img src="https://github.com/user-attachments/assets/44598316-7fd2-432b-8a9e-eccbab765b47"  width="1000"/>
</details>

<details>
  <summary><h2>🌐 API 명세서</h2></summary>
  <img src="https://github.com/user-attachments/assets/78e5917d-3bc8-43e5-add0-6e3ba315e0d3"  width="700"/>
</details>


<details>
  <summary><h2>💾 데이터베이스 (ERD)</h2></summary>
  <img src="https://github.com/user-attachments/assets/3fd00d33-0c3c-4a4f-ae01-9ff6c08db329"  width="700"/>
</details>

<details>
  <summary><h2>📅 일정 관리 (WBS)</h2></summary>
  <img src="https://github.com/user-attachments/assets/8c51f9bd-d421-4e16-864d-10c425b8a320"  width="1000"/>
</details>


<details>
  <summary><h2>📚 아키텍쳐</h2></summary>
  <img src="https://github.com/user-attachments/assets/4f0a9af1-74a1-47a5-80a2-ae9b6e249903"  width="1000"/>
</details>

<details>
  <summary><h2>💣 이슈로그</h2></summary>
  <h3>⚠️ 추론시간 장기화 문제 [AI-한줄평]</h3>
  <p><strong>문제:</strong> 한줄평 생성 시 추론시간 과다(420 시간)</p>
  <p><strong>해결:</strong> 모델 양자화를 바탕으로 시간 감소(38 시간)</p>
  
  ```
quantized_model = torch.quantization.quantize_dynamic(
    model, {torch.nn.Linear}, dtype=torch.qint8  
)
```

  <br/>
  <h3>⚠️ 문장 완성도 성능저하 문제 [AI-한줄평]</h3>
  <p><strong>문제:</strong> 원문을 한줄로 요약하면서 문장이 과도하게 길어지고 문맥의 완성도가 상당히 저하</p>
  <p><strong>해결:</strong> 추론 과정에서 원문을 일정단위로 분할요약하고 다시 합친 후 재요약하는 식으로 일부 해결</p>
  
  ```
chunks = [input_ids[i:i + 100] for i in range(0, len(input_ids), 100)]
```

  <br/>
</details>


<details>
  <summary><h2>🗨️ 후기</h2></summary>
  <p class="message">
      <strong>민정 : </strong>
      이리저리 부딪혀가며 다같이 으쌰으쌰한 3달이었습니다. 배운게 참 많아요 !!
      다들 넘 고생하셨습니다. 앞으로도 각자의 자리에서 화이팅 !! 💫
  </p>
  <p class="message">
      <strong>은진 : </strong>
  </p>
  <p class="message">
      <strong>종식 : </strong>
      처음에는 제가 끝가지 갈 수 있을까 의구심이 들었지만, 유능한 팀원들 덕분에 가능했던 것 같습니다. 모두 최종프로젝트도, 나중에 있을 취업도 화이팅입니다!
  </p>
  <p class="message">
      <strong>해린 : </strong>
      테레비들과 함께해서 즐거웠습니다. 이런저런 어려움도 팀원들 덕분에 여기까지 온 거 같아요.
      다들 너무 고생했고 마지막까지 힘내봐여 😉
  </p>
  <p class="message">
      <strong>건우 :</strong>
      우선 훌륭한 팀장님과 파트장님 덕분에 결과물을 낼 수 있었던 것 같습니다!! 다른 팀원분들도 각자 역할 잘 수행하시느라 정말 고생하셨어요. 한 사람도 빠짐없이 보고 배울 수 있었던 것 같아서 큰 행운이었던 프로젝트였고, 취업도 취업이지만 하고 싶은 일 다 잘 됐으면 좋겠습니다!! 어딜 가셔도 다들 잘할거고, 꼭꼭 항상 행복했으면 좋겠어요🍀
  </p>
  <p class="message">
      <strong>연규 : </strong>
      처음부터 끝까지 하나의 프로젝트를 함께할 수 있어서 즐거웠습니다.
      맡은 역할에 대한 책임감의 중요성을 느끼게 되었고, 남은 기간 끝까지 화이팅해요 ~ !
  </p>
  <p class="message">
      <strong>승민 : </strong>
      전체 서비스의 요구사항에 맞춰 인공지능을 탑재하는 과정이 얼마나 어렵고 복잡한지를 알 수 있었던 프로젝트였습니다. 쉽지 않은 과정이었지만 결과를 냈을때의 뿌듯함이 기억에 남습니다. 팀원분들 모두 남은 일정 유의미한 성과를 거두길 기원합니당!!
  </p>
  <p class="message">
      <strong>영빈 : </strong>
      뒤늦게 합류해서 한달밖에 함께하지 못했지만 하길 참 잘했다고 생각했습니다. 배운게 많은 한달이었습니다. 최종프로젝트도 화이팅~ 
  </p>
</details>
