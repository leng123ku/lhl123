git add .  # �������޸Ĺ��Ĺ����ļ��ύ�ݴ���
git commit -m "zengjia34"  %����ݴ����Ĵ����ύ�����زֿ⣬����עһ����zengjia34
git push origin master%�����������ļ� push������ֿ� ����ǵ�һ�μ��� -u ������� �Ͳ���  ��origin ������ֿ������ ����ʹ�������� 
���������������git remote add origin https://github.com/leng123ku/lhl123.git
%��lhl123������ֿ��ַ ����Ϊorigin������ʹ�����AAA

ͨ�������޸�һ���ļ����ҽ��ļ��ύ�����صķ�֧�������͵�Զ�̷������Ĳ������£�

git add .
git commit -m "some str"
git push

��������Ҳ���Խ���������󲽼�һ�£�
git commit -am "some str"
git push

������Ե�һ���е�git ?add .��������þ��ǽ������޸Ĺ����ļ����Ѿ�׷�ٵ��ļ���ӵ����ص��ݴ�����Ȼ��ʹ��git commit -m "str"����ݴ����Ĵ����ύ�����زֿ⣬��󽫱��زֿ�Ĵ������͵�Զ�̷������ˣ�
�ڶ�����ʵ���൱�ڵ�һ���Ľ�ϣ��������������git commit -am 'str'����ֻ���ύ�Ѿ�׷�ٹ����޸��˵��ļ���ȥ���������ļ��ͱ���ʹ�õ�һ�������



git�������
�鿴����ӡ��ύ��ɾ�����һأ������޸��ļ�
git help # ��ʾcommand��help
git show # ��ʾĳ���ύ������ git show $id
git co -- # �����������޸�
git co . # �����������޸�
git add # �������ļ��޸��ύ�������ݴ���
git add . # �������޸Ĺ��Ĺ����ļ��ύ�ݴ���
git rm # �Ӱ汾����ɾ���ļ�
git rm --cached # �Ӱ汾����ɾ���ļ�������ɾ���ļ�
git reset # ���ݴ����ָ��������ļ�
git reset -- . # ���ݴ����ָ��������ļ�
git reset --hard # �ָ����һ���ύ����״̬���������ϴ��ύ������б����޸�
git ci git ci . git ci -a # ��git add, git rm��git ci�Ȳ������ϲ���һ����������������������������������������������������������������������������git ci -am "some comments"
git ci --amend # �޸����һ���ύ��¼
git revert <$id> # �ָ�ĳ���ύ��״̬���ָ���������Ҳ�������ύ����
git revert HEAD # �ָ����һ���ύ��״̬
�鿴�ļ�diff
git diff # �Ƚϵ�ǰ�ļ����ݴ����ļ����� git diff
git diff <" style='font-size:14px;font-style:normal;font-weight:400;color:rgb(35, 35, 35);'>id1><id1> # �Ƚ������ύ֮��Ĳ���
git diff .. # ��������֧֮��Ƚ�
git diff --staged # �Ƚ��ݴ����Ͱ汾�����
git diff --cached # �Ƚ��ݴ����Ͱ汾�����
git diff --stat # �����Ƚ�ͳ����Ϣ
�鿴�ύ��¼
git log git log # �鿴���ļ�ÿ���ύ��¼
git log -p # �鿴ÿ����ϸ�޸����ݵ�diff
git log -p -2 # �鿴���������ϸ�޸����ݵ�diff
git log --stat #�鿴�ύͳ����Ϣ
tig
Mac�Ͽ���ʹ��tig����diff��log��brew install tig
Git ���ط�֧����
�鿴���л���������ɾ����֧
git br -r # �鿴Զ�̷�֧
git br # �����µķ�֧
git br -v # �鿴������֧����ύ��Ϣ
git br --merged # �鿴�Ѿ����ϲ�����ǰ��֧�ķ�֧
git br --no-merged # �鿴��δ���ϲ�����ǰ��֧�ķ�֧
git co # �л���ĳ����֧
git co -b # �����µķ�֧�������л���ȥ
git co -b # ����branch�����µ�new_branch
git co $id # ��ĳ����ʷ�ύ��¼checkout���������޷�֧��Ϣ���л���������֧���Զ�ɾ��
git co $id -b # ��ĳ����ʷ�ύ��¼checkout������������һ����֧
git br -d # ɾ��ĳ����֧
git br -D # ǿ��ɾ��ĳ����֧ (δ���ϲ��ķ�֧��ɾ����ʱ����Ҫǿ��)
 ��֧�ϲ���rebase
git merge # ��branch��֧�ϲ�����ǰ��֧
git merge origin/master --no-ff # ��ҪFast-Foward�ϲ���������������merge�ύ
git rebase master # ��master rebase��branch���൱�ڣ� git co && git rebase master && git co master && git merge
 Git��������(�����ڶ�̨�����Ͽ���ͬ��ʱ��)
git diff > ../sync.patch # ���ɲ���
git apply ../sync.patch # �򲹶�
git apply --check ../sync.patch #���Բ����ܷ�ɹ�
 Git�ݴ����
git stash # �ݴ�
git stash list # ������stash
git stash apply # �ָ��ݴ������
git stash drop # ɾ���ݴ���
GitԶ�̷�֧����
git pull # ץȡԶ�ֿ̲����з�֧���²��ϲ�������
git pull --no-ff # ץȡԶ�ֿ̲����з�֧���²��ϲ������أ���Ҫ����ϲ�
git fetch origin # ץȡԶ�ֿ̲����
git merge origin/master # ��Զ������֧�ϲ������ص�ǰ��֧
git co --track origin/branch # ����ĳ��Զ�̷�֧������Ӧ�ı��ط�֧
git co -b origin/ # ����Զ�̷�֧�������ط�֧������ͬ��
git push # push���з�֧
git push origin master # ����������֧�Ƶ�Զ������֧
git push -u origin master # ����������֧�Ƶ�Զ��(����Զ������֧�򴴽������ڳ�ʼ��Զ�ֿ̲�)
git push origin # ����Զ�̷�֧�� origin��Զ�ֿ̲���
git push origin : # ����Զ�̷�֧
git push origin : #��ɾ�����ط�֧(git br -d )��Ȼ����pushɾ��Զ�̷�֧
GitԶ�ֿ̲����
GitHub
git remote -v # �鿴Զ�̷�������ַ�Ͳֿ�����
git remote show origin # �鿴Զ�̷������ֿ�״̬
git remote add origin git@ github:robbin/robbin_site.git # ���Զ�ֿ̲��ַ
git remote set-url origin git@ github.com:robbin/robbin_site.git # ����Զ�ֿ̲��ַ(�����޸�Զ�ֿ̲��ַ) git remote rm # ɾ��Զ�ֿ̲�
����Զ�ֿ̲�
git clone --bare robbin_site robbin_site.git # �ô��汾����Ŀ�������汾�ֿ�
scp -r my_project.git git@ git.csdn.net:~ # �����ֿ��ϴ�����������
mkdir robbin_site.git && cd robbin_site.git && git --bare init # �ڷ������������ֿ�
git remote add origin git@ github.com:robbin/robbin_site.git # ����Զ�ֿ̲��ַ
git push -u origin master # �ͻ����״��ύ
git push -u origin develop # �״ν�����develop��֧�ύ��Զ��develop��֧������track
git remote set-head origin master # ����Զ�ֿ̲��HEADָ��master��֧
Ҳ�����������ø���Զ�̿�ͱ��ؿ�
git branch --set-upstream master origin/master
git branch --set-upstream develop origin/develop



