## gopm ��������ʹ��

### ��װ
> go get -v -u github.com/gpmgo/gopm

### ����ָ��
```
# �鿴��ǰ��������
gopm list
# ��ʾ������ϸ��Ϣ
gopm list -v
# �г��ļ�����
gopm list -t [file]
# ��ȡ����������Ŀ¼
gopm get -r xxx
# �����ص�ǰָ���İ�
gopm get -d xxx
# ��ȡ������$GOPATH
gopm get -g xxx
# ���������а�
gopm get -u xxx
# ��ȡ����ǰ����Ŀ¼
gopm get -l xxx
# ���е�ǰĿ¼����
gopm run
# ���ɵ�ǰ���̵� gopmfile �ļ����ڰ�����
gopm gen -v
# ���ݵ�ǰ��Ŀ gopmfile ����������ִ�� go install
gopm install -v
# ���µ�ǰ����
gopm update -v
# ������ʱ�ļ�
gopm clean
# ���뵽��ǰĿ¼
gopm bin
```