로그인
POST - /login

전체 목록 조회
GET - /api/v1/studies
{
	patientName:"",  // 환자 이름
	MRN:"",
	date:"", // 검사 날짜
	description:"", // 설명
	modailiy:"", // 검사 유형
	accession:"", // 접수 번호
	...	
}
{
	patientName:"",  // 환자 이름
	MRN:"",
	date:"", // 검사 날짜
	description:"", // 설명
	modailiy:"", // 검사 유형
	accession:"", // 접수 번호
}
...........

특정 검사 기록 뷰
GET - /api/v1/studies/{studyinstanceuid}/{seriesinstanceuid}
{
imageCnt : 10
data : [
	data1(Base64로 인코딩된 문자열),
	data2,
	data3,
	...
]
}

DicomResponseDto {
private int imageCnt;
private String[] data;
}

로컬 로그인 - mysql
데이터 읽기 전용 - oracle

