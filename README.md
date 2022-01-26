# First-Test
first repository
class Screen(object):
    width = 0
    height = 0

    @property
    def wide(self):
        return self.width

    @wide.setter
    def wide(self, width):
        self.width = width

    @property
    def high(self):
        return self.height

    @high.setter
    def high(self, height):
        self.height = height

    @property
    def resolution(self):
        return self.width*self.height


s = Screen()
s.width = 1024
s.height = 768
print('resolution =', s.resolution)
if s.resolution == 786432:
    print('测试通过!')
else:
    print('测试失败!')
